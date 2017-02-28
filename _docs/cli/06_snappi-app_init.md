---
layout: default
title: snappi-app init
permalink: /cli/snappi-app/init/
order: 5
parent: cli
---

# Defining an app

Creating snappi powered services is the first step, but the real power of Snappi is the ability to seamlessly deploy 
all services into any configured environment automatically. To do so, you'll need to create a new app, install the 
services to be deployed, and indicate which hosts you'd like the services deployed to.

```
$ snappi-app init
```

### Sample output
```sh
$ snappi-app init
  ____    _   _      _      ____    ____    ___ 
 / ___|  | \ | |    / \    |  _ \  |  _ \  |_ _|
 \___ \  |  \| |   / _ \   | |_) | | |_) |  | | 
  ___) | | |\  |  / ___ \  |  __/  |  __/   | | 
 |____/  |_| \_| /_/   \_\ |_|     |_|     |___|
                                                
Initializing Service
This utility will walk you through creating a snappi-app.json file.It only covers the most common items, and tries to 
guess reasonable defaults.Use `snappi-app install <service>` afterwards to install a service andsave it as a requirement 
in the snappi-app.json file.Press ^C at any time to quit.
name: the-batmobile
version: 1.0.0
description: Service providing access to the vast power of the batmobile!
language: javascript
git repository: https://github.com/snappi/the-batmobile.git
keywords (comma-delimited list): Na, na, na, na, na, na, na, na, BATMAN
author: Team Snappi <team@snappi.io>
license: MIT
{
    "name": "the-batmobile",
    "description": "Service providing access to the vast power of the batmobile!",
    "version": "1.0.0",
    "keywords": [
        "Na",
        "na",
        "na",
        "na",
        "na",
        "na",
        "na",
        "na",
        "BATMAN"
    ],
    "author": [
        "Team Snappi <team@snappi.io>"
    ],
    "language": "javascript",
    "license": "MIT",
    "repository": "https://github.com/snappi/the-batmobile.git"
}
```