# endUser

Kafka
1. Install Kafka
2. Go to the directory
   cd kafka_2.13-3.8.0/bin
3. Start Zookeeper
   ./zookeeper-server-start.sh ../config/zookeeper.properties
4. Start Kafka Server
   ./kafka-server-start.sh ../config/server.properties
   {
   default Port : 9092
   }
5. Create Topic With Kafka-topics
   cd ..
   bin/kafka-topics.sh --describe --topic user-topic --bootstrap-server localhost:9092
6. Produce Example Message with kafka-console-producer
   bin/kafka-console-producer.sh --topic user-topic --bootstrap-server localhost:9092
7. Consume Message with kafka-console-consume
