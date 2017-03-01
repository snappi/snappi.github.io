---
layout: default
title: snappi-app add
permalink: /cli/snappi-app/env_add
parent: cli
order: 7
---

# Add hosts to an app
Hosts are the second important piece of information that makes up a Snappi app. With the knowledge of both 
the services you wish to deploy and the hosts you wish to deploy to, the Snappi CLI can automate the deployment of 
your entire application across a distributed infrastructure.

Adding hosts is a simple command that accepts a hostname and the environment to bind it to:

```sh
$ snappi-app env <env_name> add <hostname>
```

### Additional parameters

*`--user=<username>`, `-u <username>`*

Name of the user to login to the host with

*`--key=<key>`, `-k <key>`*

Path to the SSH key used to access the host
