---
layout: default
title: app install <service>
order: 5
parent: cli
---

# Add services to an app
After you've initialized your app and created it's configuration file, you'll then have to specify which services 
should be deployed with this app. These service requirements are specified the same way they for apps as they are 
when you're creating a service - a simple command that adds the reference to your `snappi_app.json` file:

```
$ snappi app install <service name>
```