GETTING TOP 10 from the database itself WITH filtered_logs AS (
  SELECT srcip, dstip, vpn, policyid, action 
  FROM public.logs where devname='FGT1100E-Primary' and action in ('deny','blocked') and 
   eventtime >= 1684315294501269180
)

SELECT (
  SELECT ARRAY[ARRAY_AGG(srcip), ARRAY_AGG(srcip_count::text)] 
  FROM (
    SELECT srcip, COUNT(srcip) AS srcip_count
    FROM filtered_logs
    GROUP BY srcip
    ORDER BY COUNT(srcip) DESC
    LIMIT 10
  ) subquery
) AS topsrcips,
(
  SELECT ARRAY[ARRAY_AGG(dstip), ARRAY_AGG(dstip_count::text)] 
  FROM (
    SELECT dstip, COUNT(dstip) AS dstip_count
    FROM filtered_logs
    GROUP BY dstip
    ORDER BY COUNT(dstip) DESC
    LIMIT 10
  ) subquery
) AS topdstips,
(
  SELECT ARRAY[ARRAY_AGG(vpn), ARRAY_AGG(vpn_count::text)] 
  FROM (
    SELECT vpn, COUNT(vpn) AS vpn_count
    FROM filtered_logs
    GROUP BY vpn
    ORDER BY COUNT(vpn) DESC
    LIMIT 10
  ) subquery
) AS topvpns;
