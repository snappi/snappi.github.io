---
layout: default
title: environment create
order: 4
parent: cli
---

# Create an environment
Creating an environment is the first step toward publishing and deploying a set of snappi services to private, 
public, or hybrid clouds. To create an environment, type the following in the command line where `[env-name]` 
is the nickname for the environment:

```sh
$ snappi environment create [env-name]
```

OR

```sh
$ snappi env create [env-name]
```

Once created, the details of the environment will be stored in the user home directory in a hidden folder:
`~/.snappi/environments/[env-name].yml`.