# Kafka Streams to Filter Tweets


# This application will consume tweets from a Kafka Topic and send them to a different Kafka Topic.

### Useful commands


### Start Zookeeper
```
zookeeper-server-start.bat config\zookeeper.properties
```

### Start Kafka
```
kafka-server-start.bat config\server.properties
```

### Create 'Important Tweets' Topic
```
kafka-topics --zookeeper 127.0.0.1:2181 --topic important_tweets --create --partitions 3 --replication-factor 1
```

### Kafka Console Consumer
```
kafka-console-consumer --bootstrap-server 127.0.0.1:9092 --topic important_tweets --from-beginning
```
