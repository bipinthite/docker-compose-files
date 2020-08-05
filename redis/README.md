# Redis

Redis is an open-source, networked, in-memory, key-value data store with optional durability. It is written in ANSI C. The development of Redis is sponsored by Redis Labs today; before that, it was sponsored by Pivotal and VMware. According to the monthly ranking by DB-Engines.com, Redis is the most popular key-value store. The name Redis means REmote DIctionary Server.

Website: https://redis.io/

Docker Hub: https://hub.docker.com/_/redis

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker volume:
Name: `redisdata`

If don't have already this volume created, use below command to create it.
```
docker volume create redisdata
```

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```
