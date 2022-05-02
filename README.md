# ClearBrowsingData

A browser extension to clear browsing data. By default users have full control, if managed by an organization IT admins can set defaults and force settings.

## Features
- Clears browsing data on startup or when the extension icon is clicked.
- IT admins can set defaults via GPO.
- IT admins can force settings via GPO.
- Supply a list of domains to exclude from clearing.
- IT forced exclusions.

![Screenshot](/../Screenshots/ClearBrowsingData_1.png?raw=true)
![Screenshot](/../Screenshots/ClearBrowsingData_2.png?raw=true)
![Screenshot](/../Screenshots/ClearBrowsingData_3.png?raw=true)

## GPO JSON
``` JSON
{
    "ClearOnStartup": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "AppCache": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "Cache": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "CacheStorage": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "Cookies": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "Downloads": {
        "Setting": false,
        "AllowUserOverride": false
    },
    "FileSystems": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "FormData": {
        "Setting": false,
        "AllowUserOverride": false
    },
    "History": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "IndexedDB": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "LocalStorage": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "Passwords": {
        "Setting": false,
        "AllowUserOverride": false
    },
    "ServiceWorkers": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "WebSQL": {
        "Setting": true,
        "AllowUserOverride": false
    },
    "Exclusions": {
        "Setting": [
            "https://google.com",
            "https://msn.com",
            "https://yahoo.com"
        ],
        "AllowUserOverride": false
    }
}
```
