# openshift-springboot-kafka
Run zookeeper at .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties & kafka at .\bin\windows\kafka-server-start.bat .\config\server.properties

Build and Install the SpringBoot project with commandlines: mvn clean install and mvn spring-boot:run

Hit  & check logs

http://localhost:8080/jsa/kafka/producer?data=Hello World

INFO 12240 --- [io-8080-exec-10] c.j.apachekafka.services.KafkaProducer   : sending data='Hello World'
2017-06-08 13:49:47.248  INFO 12240 --- [ntainer#0-0-L-1] c.j.apachekafka.services.KafkaProducer   : received content = 'Hello World'

http://localhost:8080/jsa/kafka/producer?data=This is a SpringBoot Kafka Application

http://localhost:8080/jsa/kafka/consumer