# kafka-my-java2
- To run this project, clone the repo first.
- We also have to start kafka service from kafka folder in powershell by using the command ``` .\bin\windows\kafka-server-start.bat .\config\server.properties ```
- Then we have to start the <b>zookeeper</b> from the kafka folder using the command  ```.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties ```
- Then you can create a topic in new powershel using the command ```.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic prices```
- To run as consumer, we have to use the command ```java -cp target/mahender-kafka-api-1.0-SNAPSHOT-jar-with-dependencies.jar com.mahender.kafka.Consumer test group```
- To run as producer, we have to run the command ``` java -cp target/mahender-kafka-api-1.0-SNAPSHOT-jar-with-dependencies.jar com.mahender.kafka.ProducerSentenceRandom test```

