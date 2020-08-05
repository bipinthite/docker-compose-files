# Drools KIE Server

Docker Hub: https://hub.docker.com/r/jboss/kie-server

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```
