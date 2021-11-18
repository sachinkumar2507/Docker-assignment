FROM openjdk:8-jre-slim

WORKDIR /kafka-server

ADD kafka/ /kafka-server/

CMD ["./bin/kafka-console-producer.sh", "--broker-list server:9092", "--topic kafka-message"]