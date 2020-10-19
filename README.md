# practical-ksqldb
This repo is for doing the practical for ksqldb stuffs

# Get starting

- Step 1:

```
$ docker-compose up --remove-orphans -V
```

- Step 2:

Add table schema and data:

https://github.com/debezium/debezium-examples/blob/master/tutorial/debezium-sqlserver-init/inventory.sql

- Step 3:

```
$ curl -i -X POST -H "Accept:application/json" -H  "Content-Type:application/json" http://localhost:8083/connectors/ -d @register-sqlserver.json
```

- Step 4:

http://localhost:9021/