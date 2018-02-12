---
layout: default
title: snappi-app add-host
permalink: /cli/snappi-app/add-host
parent: cli
order: 7
---

# Add hosts to an app
Hosts are the second important piece of information that makes up a Snappi app. With the knowledge of both 
the services you wish to deploy and the hosts you wish to deploy to, the Snappi CLI can automate the deployment of 
your entire application across a distributed infrastructure.

Adding hosts is a simple command that accepts a hostname and the environment to bind it to:

```sh
$ snappi-app add-host <hostname> -e <environment_name>
```

### Required parameters

*`<hostname>`*

IP address or hostname at which the machine can be reached

*`--environment=<environment>`, `-e <environment>`*

Label to give then environment to add the host to

### Additional parameters

*`--user=<username>`, `-u <username>`*

Name of the user to login to the host with

*`--password=<password>`, `-p <password>`*

*`--key=<key>`, `-k <key>`*

Path to the SSH key used to access the host

*`--datacenter=<datacenter>`, `-d <datacenter>`*

Label for the datacenter the host exists in

*`--name=<name>`, `-n <name>`*

Friendly name to give the host for tracking
