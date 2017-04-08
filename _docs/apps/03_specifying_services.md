---
title: Specifying services
layout: default
order: 2
permalink: /apps/specifying_services/
parent: apps
---

# Specifying services to deploy
After you've successfully created your `snappi-app.json` file, you'll need to specify which services you intend to 
deploy with this app. Specifying which [snappi services](/services/what_is_a_service/) will be deployed with your 
app is a lot like [specifying service dependencies](/services/dependencies/), and can be done using a simple CLI command: 

```
$ snappi-app install <service_name>
```

**\<service_name\>** can be a reference to a service in the Snappi registry, or a reference to a git repository containing 
a `snappi-service.json` file. Once the **\<service_name\>** is validated, the reference will be appended to the 
service configuration file in the current directory. 

## Next steps
After you’ve specified which services need to be deployed with your app, it’s time to specify the details of the 
environments to which your app can be published. [Click here to learn more](/apps/provisioning_environments/).