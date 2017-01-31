---
layout: default
title: App Configuration
order: 2
permalink: /docs/app_configuration/
---

In addition to building and publishing individual services and their dependencies, Snappi can also build and ship 
entire environments containing several services. 

In order to identify and configure your app, you'll need to create a `snappi_app.json` file. Through this configuration 
file, the Snappi CLI is able to understand which services you aim to deploy, and the details of the environments you 
have available for it to be deployed to. 

## Requirements
At a minimum, a `snappi_app.json` file must have the following:

#### `name`
* All lowercase
* One word, no spaces, dashes and underscores allowed

#### `version`
* Build number of current iteration
* Numerical values, periods allowed (e.g. **x.x.x**)

#### `dependencies`
* Services to be deployed as part of the app

#### `environments`
* Key/value store of environments to deploy the app to

## All configuration options

```json
{
  "name": "avengers-app",
  "description": "Ship the avengers to stop Ultron",
  "keywords": [
    "avengers",
    "ultron",
    "sokovia"
  ],
  "version": "1.2.0",
  "author": {
    "name": "Turtle Thor",
    "email": "thor@snappi.io"
  },
  "repository": {
    "type": "Github",
    "url": "https://github.com/snappi/avengers-service.git"
  },
  "dependencies": {
    "thor.asgaard": "^1.4.2",
    "ironman.stark-enterprises": "3.0.1",
    "captain-america.winter-soldier": "2.1.5",
    "hulk.smash": "^0.1.98"
  }
}
```
