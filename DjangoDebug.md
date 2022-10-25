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
        }
        ,
        {
            "name": "FATheData",
            "python": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/FA_ENV/bin/python3",
            "type": "python",
            "request": "launch",
            "program": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/manage.py",
            "console": "integratedTerminal",
            "args": ["runserver"],
           "django": true,
           "justMyCode": true,
          }
    ]
}
