---
layout: default
title: install <service>
parent: cli
order: 3
permalink: /cli/install/
---

# Requiring other services

When working with service-oriented architecture and distributed systems, it's almost guaranteed that services will 
need to make calls to each other. Snappi supports this naturally as part of it's design flow, and all it takes is 
a simple configuration indicating which services are required before they can be referenced via dynamic RPC.

```
$ snappi install <service name>
```