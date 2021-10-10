# Kafa-Learning

Start zookeeper

./zookeeper-server-start.sh ../config/zookeeper.properties

Add below properties in server.properties

listeners=PLAINTEXT://localhost:9092
auto.create.topics.enable=false

Start broker

./kafka-server-start.sh ../config/server.properties


