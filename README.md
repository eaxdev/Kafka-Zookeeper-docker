# Kafka-Zookeeper-docker
Kafka + Zookeeper using docker with docker-compose

Example to connect from `Spring` App:

application.yml
```yml
spring.kafka.producer.bootstrap-servers=PLAINTEXT://localhost:9092"
spring.kafka.producer.key-serializer=org.apache.kafka.common.serialization.StringDeserializer"
spring.kafka.producer.value-serializer=org.springframework.kafka.support.serializer.JsonDeserializer"

spring.kafka.consumer.bootstrap-servers=PLAINTEXT://localhost:9092"
spring.kafka.consumer.group-id=group-id"
spring.kafka.consumer.auto-offset-reset=earliest"
spring.kafka.consumer.key-deserializer=org.apache.kafka.common.serialization.StringDeserializer"
spring.kafka.consumer.value-deserializer=org.springframework.kafka.support.serializer.JsonDeserializer"
spring.kafka.consumer.properties.spring.json.trusted.packages=*"
```
