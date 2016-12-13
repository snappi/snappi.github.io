---
layout: default
title: The snappi.json file
permalink: /docs/snappi_configuration/
---

The `snappi.json` is the most important piece of any snappi enabled service. Through this simple configuration file,
the Snappi CLI is able to understand everything about your service as well as the services it depends on. Some of the 
notable pieces of information included in the file include:

1. Package name and version number for your service allowing others to reference and consume it
2. Description, documentation, and other meta information about the service so it can be discovered and shared
3. Names and versions of packages that your service is dependent on. 

## Requirements
At a minimum, a `snappi.json` file must have the following:

#### `name`
* All lowercase
* One word, no spaces, dashes and underscores allowed

#### `version.name`
* Unique version name
* All lowercase
* One word, no spaces, dashes and underscores allowed

#### `version.number`
* Build number of current iteration
* Numerical values, periods allowed (e.g. **x.x**)

```json
{
  "name": "my-microservice",
  "version": {
    "name": "jellybean",
    "number": "1.2"
  }
}
```

### What's the difference between `name` and `version.name`?
The `name` of your service is unique to the service overall, and is the name that will be searchable if and when your 
service is published publicly. The `version.name` is a package identifier cooresponding to the current integration 
contract for your service. If you wish to publish "breaking" changes to your service, you'll be forced to change the 
`version.name` so integrating developers don't accidentally break their integration with your service.

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
  "version": {
    "name": "batman-begins",
    "number": "1.2.0"
  },
  "author": {
    "name": "Turtle Batman",
    "email": "batman@snappi.io"
  },
  "repository": {
    "type": "Github",
    "url": "https://github.com/snappi/batman-service.git"
  },
  "bugs": {
    "url": "https://github.com/snappi/batman-service/issues"
  },
  "dependencies": {
    "superman-service.superman-returns": "^2.0.0",
    "theflash-service.flashpoint": "^1.0.0"
  }
}
```
