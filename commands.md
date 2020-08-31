Run the docker compose:
```
docker-compose up
```

Run in detatched mode:
```
docker-compose up -d
```

Stop the docker-compose :
```
docker-compose stop
```

To build a service run
```
docker-compose build <service>
```

Get to the service bash 
```
docker-compose exec <service> bash
```

Create random table in postgre:
```
create table test_table as select random_column from 
(SELECT generate_series(1,10) AS id,md5(random()::text) AS random_column)s;
```


The agenda
1. Docker file instroduction
2. Presenting the services
3. Running the pgadmin 
4. Connecting the postgres 
6. Running the jupyter from Dockerfile
7. Connecting to postgres from jupyter
8. Mapping environment variables