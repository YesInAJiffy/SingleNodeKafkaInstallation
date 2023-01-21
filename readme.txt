For details, please refer the below video
https://www.youtube.com/watch?v=7qurUlZUayA


COMPOSE THE DOCKER
docker-compose up -d

GO TO THE SHELL (inside the docker)
docker exec -it broker bash

CREATE TOPIC
kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092

CREATE PRODUCER
kafka-console-producer --topic quickstart-events --bootstrap-server localhost:9092

CREATE CONSUMER
kafka-console-consumer --topic quickstart-events1 --from-beginning --bootstrap-server localhost:9092


STOP THE BROKER
docker-compose down
