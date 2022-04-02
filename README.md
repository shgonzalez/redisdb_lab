# redisdb_lab

Docker compose file for redis and redis insight, graphical user interface for redis. In this configuration, Redis Insight is reachable from the outside of the Docker host, just make sure your firewall has opened the 8001 port.

![diagram](/redisdblab.png)

Start containers:

```bash
docker-compose up -d 
```

Optional, add database using API

```bash
curl -X POST -H 'Content-Type: application/json' --data '@myredisdb.json' http://localhost:8001/api/instance/
```

You can navigate to [http://localhost:8001](http://localhost:8001) and add your redis databases
