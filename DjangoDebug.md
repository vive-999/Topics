{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "console": "integratedTerminal",
            "justMyCode": true
        },
        {

            "name": "FATheData",
            
            "python": "/home/vivekraj/FAENVAGAIN/bin/python3",
            
            "type": "python",
            
            "request": "launch",
            
            "program": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/manage.py",
            
            "console": "integratedTerminal",
            
            "args": ["runserver","9090"],
            
            "django": true,
            
            "justMyCode": true,
            
            },
        {

            "name": "API_Dashboard_defpage",
            
            "python": "/home/vivekraj/FAENVAGAIN/bin/python3",
            
            "type": "python",
            
            "request": "launch",
            
            "program": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/api/modules/dashboard_defpage_utils.py",
            
            "console": "integratedTerminal",
            
            "args": ["accept", "passthrough", "202.154.167.3" ,"wazuh-archives-4.x-2022.12.01"],
            
            "django": true,
            
            "justMyCode": true,
            
            },
        {

            "name": "API_Dashboard_Search",
            
            "python": "/home/vivekraj/FAENVAGAIN/bin/python3",
            
            "type": "python",
            
            "request": "launch",
            
            "program": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/api/modules/dashboard_search_utils.py",
            
            "console": "integratedTerminal",
            
            "args": ["accept" ,"passthrough" ,"Corporate_Firewall" ,"30_minutes", "nan" ,"nan" ,"wazuh-archives-4.x-2022.12.01" ,"0", "202.154.167.3"],
        
            "justMyCode": true,
            
            },

    ]
}
