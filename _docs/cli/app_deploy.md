---
layout: default
title: app deploy <env>
order: 8
parent: cli
---

# Deploy an environment
Once an environment has been created and configured to include a set of Snappi services and target hosts, the Snappi 
CLI can handle the entire application deployment! To deploy an application, type the following in the command line:

```sh
$ snappi app deploy <env>
```

## What does deployment do?
The Snappi CLI automates the deployment of a potentially extensive microservice architecture, so it's very reasonable 
to wonder how this can be accomplished and what steps are happening under the hood. Below is a list of functions 
performed by the deployment command, and you're welcome to step through the full source code for the project at your 
liesure:

### Dependency mapping
Snappi services specify their own dependencies, so it's entirely possible (and even highly probable) for two 
services to share the same service as a dependency. To maximize the efficiency of the deployed application, 
the Snappi CLI maps out these dependencies, determines which need to be deployed first, and eliminates redundency.

### Docker image building
If docker images for the environment's services haven't already been created, Snappi handles their creation 
automatically and ensures they are properly configured for the deployment target.

### Push Docker images to target hosts
Once docker images have been properly provisioned and configured, the images are then distributed evenly amongst the 
target hosts configured with the environment.

### Create load balancers
In order to distribute requests to active service instances, Snappi creates load balancers for each unique service to 
route requests accordingly.

### Configure RPC stubs
One of the most important features of Snappi is the ability to connect services to each other at deploy time. Once the 
load balancers for each service have been created, Snappi can create RPC stubs referencing the proper load balancers 
and inject them into services that need to know where their peers are.
