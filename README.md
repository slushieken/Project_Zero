# AWS exercise for Cartel Project Zero - Infrastructure Code

This GitHub repo will hold the CloudFormation infrastructure code for Cartel Project Zero.

# Task:

Implement CD pipeline on AWS with Zero Downtime deploy of a single http service.

## Project Zero Requirements

* implement on AWS

* Zero Downtime service deployable simple http service with Continuous Integration pipeline

* a setup that will deploy a new version of the service after a git push.

* Some thought should also be put into making the service highly available and scalable in general.

* Automatization of the required/selected infrastructure is not required.

* Service should be dynamic, in other words, not just a static site but something that does something simple. You can use technologies to your liking.

* When new version service is deployed, it should not respond to traffic for 15 seconds, to simulate the startup time of the service.

* When deploying the service, the new version should be in a new environment, it cannot share processes with the old version.

## Use case:

* When I push a change to git, event is triggered I want the new version of the service deployed within 1 minute and I can use it without any downtime for me even during deploy procedure.

## Solution:

ECS Containers
