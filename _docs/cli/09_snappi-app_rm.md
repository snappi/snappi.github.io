---
layout: default
title: snappi-app rm
permalink: /cli/snappi-app/env_rm
parent: cli
order: 8
---

# Remove host from environment
To remove a host from an environment, simply indicate the hostname you wish to remove and which environment it should 
be removed from:

```sh
$ snappi-app rm <hostname> --environment="<env_name>"
$ snappi-app rm <hostname> -e "<env_name>"
```