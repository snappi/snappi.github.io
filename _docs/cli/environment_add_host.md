---
layout: default
title: environment add [host]
parent: cli
order: 6
---

# Add host to environment
Hosts are the second important piece of information that makes up a Snappi environment. With the knowledge of both 
the services you wish to deploy and the hosts you wish to deploy to, the Snappi CLI can automate the deployment of 
your entire application across a distributed infrastructure.

To add a host to a previously created environment, type the following into the command line:

```sh
$ snappi environment [env-name] add [hostname]
```

OR 

```sh
$ snappi env [env-name] add [hostname]
```

Where `[env-name]` is the name of your environment, and `[hostname]` is the address of the machine you wish to deploy 
to. You may also specify the following two optional arguments in the command:

##### `--user=[username]`, `-u [username]`
Name of the user to login to the host with

##### `--key=[key]`, '-k [key]'
Path to the SSH key used to access the host