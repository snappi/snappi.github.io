---
title: Creating a service
layout: default
order: 1
permalink: /services/creating/
parent: services
---

# Creating Services
Creating Snappi enabled services is a lot like the creation of libraries and microservices when left up to your own devices. 
In fact, the interface requirements were left intentionally lean so as to allow developers to use their own code styles 
and development habits without being hampered by obnoxious dependencies.

As described in the [previous document](/services/what_is_a_service/), the first step to creating a snappi service is 
to create your `snappi-service.json` file outlining the configuration options for your service. To aid this process, 
we've created an initialization command that will walk you through the process and generate your `snappi-service.json` 
file. 

```
$ snappi-service init
```

Once the wizard is complete, the CLI will place the generated `snappi-service.json` file into the directory in which 
the command was kicked off. After that, you're ready to [specify which services your new one is dependent upon](/services/dependencies).