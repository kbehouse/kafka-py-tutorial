# Kafka-py-tutorial

## Start confulent kafka 

```
docker-compose up
```

## Run

Consumer

```
# python3 consumer.py localhost:29092 [group_id] [topic] 
python3 consumer.py localhost:29092 aa foobar
```


Producer
```
# py producer.py localhost:29092 [topic]
py producer.py localhost:29092 foobar
```

## Kafka Tool

Topic List

```
docker exec -it broker kafka-topics --list --bootstrap-server localhost:29092
```

Consumer in docker

```
docker exec -it broker kafka-console-consumer --bootstrap-server localhost:29092  --from-beginning --topic foobar
```

## Refer

* Docker compose: https://kafka-tutorials.confluent.io/join-a-stream-to-a-table/ksql.html
* Kafka Python: https://github.com/confluentinc/confluent-kafka-python
