---
layout: page
title: Snappi Init
parent: cli
order: 0
permalink: /docs/cli/init/
---

### Initializing a Snappi App
Open a terminal, then create a folder for your new Snappi app and navigate into it. This is where your app will be created.
```sh
$mkdir my-new-snappi-app
$cd my-new-snappi-app
```

Run Snappi init to create the skeleton for your new app. It will prompt you for things like what you would like to name your app, keywords to describe it, the Snappi plugins that you would like to use, and so on.
``` sh
$snappi init
```

You will notice that a snappi.json file was created in your project directory and is filled out according to the options that you specified. It will look like this:
```json
"name": "my-new-snappi-app",
"description": "my new snappi app!",
"version": "0.0.0",
"keywords": ["new", "fresh", "off-the-chain", "easy", "microservices"],
"author": {
    "name": "Snappi the Turtle",
    "email": "snappiTheTurtle@snappi.io"
},
"license": "MIT",
"repository": {
    "type": "GitLab",
    "url": "https://gitlab.com/SnappiPlatform/snappi-cli"
},
"bugs": {
    "url": "https://gitlab.com/SnappiPlatform/snappi-cli/issues"
},
"dependencies": {
    
}
```