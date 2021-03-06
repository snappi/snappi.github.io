---
layout: default
title: snappi-service init
parent: cli
order: 2
permalink: /cli/snappi-service/init/
---

# Creating a `snappi-service.json` file
A configuration file for your service can always be created through any simple text editor, but the CLI also comes with 
a handy function that walks through the creation process and generates a `snappi-service.json` file for you. To use this tool, 
simply type:

```
$ snappi-service init
```

This will initiate a command line questionnaire that will conclude with the creation of a `snappi.json` file in the 
directory in which you initiated the command.

### Sample output
```
$ snappi-service init
This utility will walk you through creating a snappi.json file.
It only covers the most common items, and tries to guess reasonable defaults.

Use `snappi-service install <service>` afterwards to install a service and
save it as a requirement in the snappi-service.json file. 

Press ^C at any time to quit.
name: (test-service) 
version: (1.0.0) 
description: My first Snappi service
language: javascript
main file: (index.js) 
git repository: https://github.com/snappi/test-service
keywords: snappi, test, service
author: Snappi
license: (ISC) 
About to write to /path/to/test-service/snappi.json:

{
  "name": "test-service",
  "version": "1.0.0",
  "description": "My first Snappi service",
  "language": "javascript",
  "main": "index.js",
  "repository": {
    "type": "git",
    "url": "git+https://github.com/snappi/test-service.git"
  },
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