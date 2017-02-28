---
title: Publishing services
layout: default
order: 3
permalink: /services/publishing/
parent: services
---

# Publishing services <small>(coming soon)</small>
Snappi services can be leveraged and installed by referencing a git repository hosting the service, but services will 
soon be publishable and accessible via the Snappi registry. Once released, this registry will allow users to login, 
publish their services both publicly and privately, share services with friends and colleagues, and browse for 
open-source services contributed by the community. 

The Snappi team has made a prototype of this registry accessible via the CLI, but for now only our team can publish 
services. If you're interested in publishing a service to this registry then [let us know](mailto:team@snappi.io), and 
if you'd like to see what services we've made available then feel free to [use the search command](/services/search) 
in the CLI. Once the feature is public, anyone will be able to publish services using the command from a directory 
housing a valid `snappi-service.json` file:

```
$ snappi-service publish
```