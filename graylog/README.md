# Graylog

Graylog is a centralized logging solution that allows the user to aggregate and search through logs. It provides a powerful query language, a processing pipeline for data transformation, alerting abilities and much more. It is fully extensible through a REST API. Add-Ons can be downloaded from the Graylog Marketplace.

Website: https://www.graylog.org/

Docker Hub: https://hub.docker.com/r/graylog/graylog

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker volumes:
Name: `graylog_journal`

If don't have already this volume created, use below command to create it.
```
docker volume create graylog_journal
```

Name: `esdata`

If don't have already this volume created, use below command to create it.
```
docker volume create esdata
```

If you're using Docker Stack to run the containers, create overlay network,

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```
