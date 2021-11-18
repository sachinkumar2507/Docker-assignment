# Kafka Producer and Consumer using docker and docker-compose example

- Running the zookeeper on the docker container

### Installation

Install docker and docker-compose from official docker website and run the below commands

#### zookeeper docker images and run it inside the kafka-network

```
$ docker-compose up -d
```

#### Creating topic

```
docker exec server ./bin/kafka-topics.sh --bootstrap-server server:9092 --create --partitions 1 --replication-factor 1 --topic quickstart
```

#### Running producer and consumer in different terminals

```
docker exec -it server bash producer
docker exec -it server bash consumer

```

