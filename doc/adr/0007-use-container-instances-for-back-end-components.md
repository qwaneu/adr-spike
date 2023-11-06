# 7. use container instances for back end components

Date: 2023-11-06

## Status

Accepted

## Context

We have some back end components that need to be deployed independently. They are java or kotlin based component based on the spring framework. We think that function apps may be a bit slow to load (because of spring) and we do not need the scaleability function apps bring. 

We want to be prepared for more scaleability, potentially moving to k8s or container apps.

## Decision

We deploy the back end components as container instances, the cheapest way to deploy containrs. 

## Consequences

We need to build and scan container images. We need to monitor base container updates. Deployment is a breeze. We can (almost) replicate the production environment locally, using docker compose files. 

De are prepared to move on to more sophisticated container application environments.


