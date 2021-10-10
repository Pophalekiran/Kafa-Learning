# Kafa-Learning

Start zookeeper

./zookeeper-server-start.sh ../config/zookeeper.properties

Add below properties in server.properties

listeners=PLAINTEXT://localhost:9092

auto.create.topics.enable=false

Start broker

./kafka-server-start.sh ../config/server.propertiesy

How to create topic

./kafka-topics.sh --create --topic test-topic -bootstrap-server localhost:9092 --replication-factor 1 --partitions 4

Produce messages on topic

./kafka-console-producer.sh --topic test-topic --boootstrap-server localhost:9092 

Consumer to consume messages

./kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test-topic --from-beginning





