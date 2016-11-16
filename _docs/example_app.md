---
layout: page
title: Example App
permalink: /docs/example_app/
order: 2
---

### Initializing a Snappi App
Create your project directory, then using the Snappi CLI, run the following
```sh
$snappi init
```
You'll notice that a `snappi.json` file was added to the project directory. This is where you will declare the plugins that you would like to use in your app. When you create your plugins, Snappi will look here to find what services you would like to dockerize.

##### Adding a Plugin to a Snappi app
