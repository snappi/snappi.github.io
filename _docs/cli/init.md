---
layout: default
title: init
parent: cli
order: 2
permalink: /docs/cli/init/
---

# Creating a `snappi.json` file
A configuration file for your service can always be created through any simple text editor, but the CLI also comes with 
a handy function that walks through the creation process and generates a `snappi.json` file for you. To use this tool, 
simply type:

```
snappi init
```

This will initate a command line questionnaire that will conclude with the creation of a `snappi.json` file in the 
directory you initiated the command.

### Sample output
```
$ snappi init
This utility will walk you through creating a snappi.json file.
It only covers the most common items, and tries to guess reasonable defaults.

Use `snappi require <service>` afterwards to install a service and
save it as a requirement in the snappi.json file. 

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