# redisdb_lab

![diagram](/redisdblab.png)

Start containers:

```bash
docker-compose up -d 
```

Optional, add database using API

```bash
curl -X POST -H 'Content-Type: application/json' --data '@myredisdb.json' http://localhost:8001/api/instance/
```
