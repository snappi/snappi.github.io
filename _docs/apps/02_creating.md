---
title: Creating an app
layout: default
order: 1
permalink: /apps/creating/
parent: apps
---

# Creating apps
Creating snappi apps is very similar to [creating services](/services/creating) in that it simply involves the curation 
of a formatted configuration file, appropriately named `snappi-app.json`. As with the service configuration, the Snappi 
CLI contains a helpful initialization command that will walk you through the process of generating your `snappi-app.json` 
file:

```
$ snappi-app init
```

## Next steps
Once the initial configuration is complete, you're ready to start [specifying services to deploy](/apps/specifying_services). 