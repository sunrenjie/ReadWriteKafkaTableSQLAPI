# ReadWriteKafkaTableSQLAPI
Read from Kafka and aggregate data using Table and SQL API, writing back to Kafka

## How to run the program

#### Start a kafka cluster
Then Create an input and an output topic. For example, "ReadWriteKafkaTableSQLAPI-input" and "ReadWriteKafkaTableSQLAPI-output".
--read-topic test --write-topic test --bootstrap.servers localhost:9092 --group.id test-consumer-group

#### Run the random event generator
Shall modify it to use input topic and the kafka broker (defaults to localhost:9292).

#### Run ReadWriteKafkaTableSQLAPI
Command line arguments: "--read-topic ReadWriteKafkaTableSQLAPI-input --write-topic ReadWriteKafkaTableSQLAPI-output --bootstrap.servers localhost:9092 --group.id ReadWriteKafkaTableSQLAPI".
