# Changing datatype of Columns using sed editor.
1.**character varying(*) -> text**  
2.**integer  -> bigint**

1. sed -i 's/character varying(\([0-9]\+\))/text/g' your_backup_file.sql  
2. sed -i 's/integer/bigint/g' your_backup_file.sql

