```docker compose up
docker exec -it broker /bin/bash
kafka-topics --bootstrap-server broker:9092 --delete --topic messages
kafka-topics --create --bootstrap-server broker:9092 --topic messages
kafka-topics --describe --bootstrap-server broker:9092 --topic messages

pip3 install kafka-python 
python producer.py
python consumer.py
```
