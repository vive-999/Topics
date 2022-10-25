 // Use IntelliSense to learn about possible attributes.
// Hover to view descriptions of existing attributes.
// For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387

###Add the following json to the configuration List of the VSCode debug console.

{
            "name": "FATheData",                          ###A name for the debugg file
            "python": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/FA_ENV/bin/python3",           ###File location of python to be used from
            "type": "python",                                                                           ###Type of programing/file
            "request": "launch",                                                                        
            "program": "/home/vivekraj/FILEEXCHANGE/fw_analyzer_dashboard/manage.py",                  ### location of manage.py
            "console": "integratedTerminal",                                                           ###where to show the output
            "args": ["runserver"],                                                                     ####Arguments after the command
           "django": true,
           "justMyCode": true,
          }





