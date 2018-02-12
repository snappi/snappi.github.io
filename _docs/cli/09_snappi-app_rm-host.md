---
layout: default
title: snappi-app rm-host
permalink: /cli/snappi-app/rm-host
parent: cli
order: 8
---

# Remove host from environment
To remove a host from an environment, simply indicate the hostname you wish to remove and which environment it should 
be removed from:

```sh
$ snappi-app rm-host <hostname> -e <environment_name>
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
