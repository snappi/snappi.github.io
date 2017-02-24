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
$ snappi app init
```

### Sample output
```
$ snappi app init
This utility will walk you through creating a snappi_app.json file.
It only covers the most common items, and tries to guess reasonable defaults.

Use `snappi app require <service>` afterwards to install a service and
save it as a requirement in the snappi_app.json file. 

Press ^C at any time to quit.
name: (test-app) 
version: (1.0.0) 
description: My first Snappi app
keywords: snappi, test, service
author: Snappi
About to write to /path/to/test-service/snappi_app.json:

{
  "name": "test-app",
  "version": "1.0.0",
  "description": "My first Snappi app",
  "keywords": [
    "snappi",
    "test",
    "service"
  ],
  "author": "Snappi",
  "license": "ISC"
}


Is this ok? (yes)
```