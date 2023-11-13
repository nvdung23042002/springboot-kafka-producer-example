                                    APACHE KAFKA
Apache Kafka is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

## Link install Apache Kafka Turorial
- `https://www.digitalocean.com/community/tutorials/how-to-install-apache-kafka-on-ubuntu-20-04`


## Start Kafka Server
- `sudo systemctl start kafka.service`


## Show list of topic
- `/home/kafka/kafka/bin/kafka-topics.sh --list --bootstrap-server localhost:9092`


## Create Kafka Topic
- `/home/kafka/kafka/bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example`
- `/home/kafka/kafka/bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example_json`


## Publish to the Kafka Topic via Console
- `/home/kafka/kafka/bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example`
- `/home/kafka/kafka/bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example_json`
