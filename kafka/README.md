# Kafka

Apache Kafka is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

Website: http://kafka.apache.org/

Docker Hub: https://hub.docker.com/r/wurstmeister/kafka

## Pre-requisites

Before running this docker-compose file, you would need to first create below docker resources.

### Docker Network:
Name: `back-tier`

If don't have already this network created, use below command to create it.
```
docker network create back-tier --driver overlay
```
