# MongoDB

MongoDB is a cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas. MongoDB is developed by MongoDB Inc. and licensed under the Server Side Public License.

https://www.mongodb.com/


## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker volume:
Name: `mongodata`

If don't have already this volume created, use below command to create it.
```
docker volume create mongodata
```

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```
