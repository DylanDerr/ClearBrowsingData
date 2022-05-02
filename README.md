# ClearBrowsingData

A browser extension to clear browsing data. By default users have full contorl, if managed by an organization IT admins can set defaults for force settings.

## Features
- Clears browsing data on startup
- IT can set defaults
- IT can force settings
- Retrieve configs using QR code / file

## GPO Options
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
