```
docker-compose up -d

docker exec -it kafka kafka-console-producer --broker-list kafka:9092 --topic test
docker exec -it kafka kafka-topics --bootstrap-server kafka:9092 --list
docker exec -it kafka kafka-console-consumer --bootstrap-server kafka:9092 --topic global_log_topic --from-beginning

```


docker exec -it kafka /bin/bash
kafka-console-producer --broker-list kafka:9092 --topic test
kafka-topics --bootstrap-server kafka:9092 --list
