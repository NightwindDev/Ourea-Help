# Ourea

## What is Ourea?
Ourea is a "package manager"-like app for non-jailbroken devices. It is similar to Cydia where you can install tweaks for the device, although with Ourea, you install Shortcuts instead.

## How Do I Set-Up a Repo?
It is very straight-forward to set-up a repo to host your Shortcuts!

1) Create a `repo.json` file wherever you want to set-up your repo. It can be on GitHub or it could be on your personal website.
2) Follow this pattern to plan out your repo:
```json
[
     {
        "name": "The shortcut's name",
        "author": "The author of the shortcut",
        "version": "The latest version of the shortcut",  
        "description": "Short description of the shortcut",
        "longDescription": "Link to the website with the long description of the shortcut",
        "download": "Link to download the shortcut, usually starts with https://www.icloud.com/shortcuts/...",
        "compatibility": [
            "Minimum compatible version of iOS, for example 15.0",
            "Maximum compatible version of iOS, for example 15.4"
        ],
        "icons" : {
            "shortcut": "The URL to the icon of the shortcut",
            "author": "The URL to the profile picture of the author",
            "banner": "Link to the shortcut banner"
        },
        "screenshots" : [
            "Link to a screenshot showcasing the shortcut 1",
            "Link to a screenshot showcasing the shortcut 2",
            "Link to a screenshot showcasing the shortcut 3",
            "Link to a screenshot showcasing the shortcut 4"
        ],
        "olderVersions": {
            "Older version number 1": "Link to download older version 1",
            "Older version number 2": "Link to download older version 2"
        }
    }
]
```

An example Shortcut could look like this:
```json
[
     {
        "name": "Test Shortcut",
        "author": "Nightwind",
        "version": "1.0",  
        "description": "This is a test shortcut",
        "longDescription": "https://google.com",
        "download": "https://www.icloud.com/shortcuts/10294857a8481jsw1919358",
        "compatibility": [
            "13.0",
            "15.4"
        ],
        "icons" : {
            "shortcut": "https://avatars.githubusercontent.com/u/81449663?v=4",
            "author": "https://avatars.githubusercontent.com/u/81449663?v=4",
            "banner": "https://avatars.githubusercontent.com/u/81449663?v=4"
        },
        "screenshots" : [
            "https://avatars.githubusercontent.com/u/81449663?v=4",
        ],
        "olderVersions": {
            "0.9": "https://icloud.com/shortcuts/18394fuirg87456t7f7e8g98",
            "0.8.1": "https://icloud.com/shortcuts/uefjvd8ve7717348heve354556"
        }
    }
]
```
