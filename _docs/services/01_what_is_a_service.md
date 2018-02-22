---
title: What is a service?
layout: default
permalink: /services/what_is_a_service/
order: 0
parent: services
---

# What is a Snappi Service?
Services are the lifeblood of Snappi, and represent the individual modules and components that developers create and 
use as part of their applications. It's our goal to make microservice development as easy as creating 
libraries and SDKs - thus simplifying and empowering service-oriented development.

Creating and configuring individual services is a simple, but crucial part of leveraging Snappi. In ensuring that 
services adhere to the same interface and configuration guidelines, Snappi is able to automate deployment, scaling, 
and interprocess communication.

In order to identify and configure your service, you'll need to create a `snappi-service.json` file. Through this 
simple configuration file, the Snappi CLI is able to understand everything about your service as well as the services it 
depends on. Some of the notable pieces of information included in the file include:

1. Package name and version number for your service, allowing others to reference and consume it
2. Description, documentation, and other meta information about the service - so it can be discovered and shared
3. Names and versions of other services on which your service is dependent

## Requirements
At a minimum, a `snappi-service.json` file must have the following:

#### `name`
* All lowercase
* One word: without spaces, dashes, or underscores

#### `version`
* Build number of current iteration
* Numerical values: periods are allowed (e.g. **x.x.x**)
* Follows [semver spec](https://docs.npmjs.com/getting-started/semantic-versioning)

```json
{
  "name": "my-microservice",
  "version": "1.2.0"
}
```

## All configuration options

```json
{
  "name": "batman-service",
  "description": "Call and spawn batman instances across gotham",
  "keywords": [
    "batman",
    "gotham",
    "dark",
    "knight",
    "detective"
  ],
  "version": "1.2.0",
  "author": {
    "name": "Turtle Batman",
    "email": "batman@snappi.io"
  },
  "repository": {
    "type": "Github",
    "url": "https://github.com/snappi/batman-service.git"
  },
  "services": {
    "superman-service": "2.0.0",
    "theflash-service": "1.0.0"
  }
}
```

## Creating your first service
Now that you understand what a Snappi Service is, you’re ready to [create your own](/services/creating/)!
