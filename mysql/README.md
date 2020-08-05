# MySQL

MySQL is the world's most popular open source database. Whether you are a fast growing web property, technology ISV or large enterprise, MySQL can cost-effectively help you deliver high performance, scalable database applications.

Website: https://www.mysql.com/

Docker Hub: https://hub.docker.com/_/mysql

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker volume:
Name: `mysqldata`

If don't have already this volume created, use below command to create it.
```
docker volume create mysqldata
```

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```

## Bootstrap data:

When a container is started for the first time, a new database with the specified name will be created and initialized with the provided configuration variables. Furthermore, it will execute files with extensions `.sh`, `.sql` and `.sql.gz` that are found in `./initdb`. Files will be executed in alphabetical order. You can easily populate your mysql services by mounting a SQL dump into that directory and provide custom images with contributed data. SQL files will be imported by default to the database specified by the `MYSQL_DATABASE` variable.
