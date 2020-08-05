# OpenLDAP

OpenLDAP Software is an open source implementation of the Lightweight Directory Access Protocol.

Website: http://www.openldap.org/

Docker Hub: https://hub.docker.com/r/osixia/openldap/

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker volume:
Name: `ldapdata`

If don't have already this volume created, use below command to create it.
```
docker volume create ldapdata
```

Name: `slapdconfig`

If don't have already this volume created, use below command to create it.
```
docker volume create slapdconfig
```

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```

Name: `front-tier`

If don't have already this network created, use below command to create it.
```
docker network create front-tier --driver overlay
```
