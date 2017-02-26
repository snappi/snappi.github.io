---
title: What is an app?
layout: default
permalink: /apps/what_is_an_app/
order: 0
parent: apps
---

# What is a Snappi App?
Snappi apps are the containment structure that dictates which services you plan on using, and where you plan on 
deploying them to. As such, apps consist of two parts:

1. A collection of snappi enabled services, and
2. Environment definitions - collections of hosts that the specified services can be deployed to

In order to identify and configure your app, you'll need to create a `snappi-app.json` file. Through this configuration 
file, the Snappi CLI is able to understand which services you aim to deploy, and the details of the environments you 
have available for it to be deployed to. 

# Requirements
At a minimum, a `snappi-app.json` file must have the following:

#### `name`
* All lowercase
* One word, no spaces, dashes and underscores allowed

#### `version`
* Build number of current iteration
* Numerical values, periods allowed (e.g. **x.x.x**)
* Follows [semver spec](https://docs.npmjs.com/getting-started/semantic-versioning)

#### `services`
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
  "services": {
    "asgaard": "^1.4.2",
    "stark-enterprises": "3.0.1",
    "winter-soldier": "2.1.5",
    "hulk": "^0.1.98"
  },
  "environments": {
    "local": [
      {
        "host": "127.0.0.1",
        "options": {}
      }
    ],
    "production": [
      {
        "host": "12.34.56.78",
        "options": {}
      },
      {
        "host": "23.45.67.89",
        "options": {}
      }
    ]
  }
}
```
