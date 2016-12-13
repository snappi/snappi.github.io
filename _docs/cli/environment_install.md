---
layout: default
title: environment install [service]
order: 5
parent: cli
---

# Add services to an environment
One of the two major components of a Snappi environment are the Snappi-powered services that it includes. 
Armed with the knowledge of these services, the Snappi CLI is able to seamlessly deploy your entire 
application architecture to any number of public or private hosts.

To add a service to your environment, install it the same way you would install a depedency to a service:

```sh
$ snappi environment [env-name] install [service-url]
```

OR

```sh
$ snappi env [env-name] install [service-url]
```

where `[env-name]` is the name of the environment, and `[service-url]` is the URL to the github repository containing 
the service. 

_Note: in the near future, you'll be able to search for and reference services simply by name if they've been published 
to Snappi's registry. Keep an eye out for an update with more details!_