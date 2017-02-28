---
title: Specifying dependencies
layout: default
order: 2
permalink: /services/dependencies/
parent: services
---

# Specifying service dependencies
Needing to specify dependencies for microservices can seem like a strange concept at first, but the ability for services 
to be aware of what peers they depend on is a powerful feature. Armed with this awareness, the Snappi CLI is able to 
deploy and orchestrate a service as well as all it's dependencies using a single command. 

To identify and leverage additional services as dependencies of your own, start with the following CLI command:

```
$ snappi-service install <service_name>
```

**\<service_name\>** can be a reference to a service in the Snappi registry, or a reference to a git repository containing 
a `snappi-service.json` file. Once the **\<service_name\>** is validated, the reference will be appended to the 
service configuration file in the current directory. 

## Injecting service references
After updating your `snappi-service.json` file to reflect the desired dependencies, these dependencies can be injected 
directly into your own microservice. The means of injecting service references is unique in each language, and the 
Snappi CLI is constantly being updated to ensure we support every server-side language. 

The below is a brief example of how you'd inject a *userManagement* microservice into a node.js service:

```js
var express = require('express');

exports.init = function(userManagement) {
    
    const app = express();
    
    app.post('/login', function(req, res) {
        userManagement.login(req.body.username, req.body.password)
            .then(function(result) {
                res.status(200).send(result);
            });
    });
    
    app.listen(8080);
    
};
```

**Alpha release notes**: *Throughout our alpha release, we'll be constantly adding support for a variety of different 
languages. [Click here]() to see what languages we support, and [don't hesitate to reach out](mailto:team@snappi.io) 
if you have any requests!*

## Next steps
After you've successfully installed and injected the services you need, you're ready to publish your service! Check out 
our guide on [publishing services](/services/publishing) to learn how yours can be shared with your team or the community.