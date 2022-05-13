Run Kafka Cluster

```sh
docker-compose up -d
```

```sh
while ! nc -z localhost 29092; do
  sleep 1
  echo "Waiting on Kafka to launch on 29092..."
done
```

Intract with Kafka Cluster

```sh
docker-compose exec kafka bash
```
