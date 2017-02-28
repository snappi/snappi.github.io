---
layout: default
title: snappi config
parent: cli
order: 0
permalink: /cli/snappi/config/
---

# Configuring Snappi
There are a variety of configuration options that will be added to Snappi over time. To accommodate these needs, the 
CLI includes a shortcut command to modify these configuration options as a key/value store:

```
$ snappi config <key> <value>
```

## All configuration options

#### `user.email`
The email address of the user currently using the CLI. Used to identify the user and login to the public registry.

#### `user.name`
The name of the user currently using the CLI. 