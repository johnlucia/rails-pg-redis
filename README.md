# Rails/Postgres/Redis/Docker Starter Kit

Create the bundle cache volume if it doesn't already exist:
```
docker volume create ruby-bundle-cache
```
Spark it up:
```
docker compose up -d
``` 
Create the database if it doesn't already exist:
```
docker compose run --service-ports web bash
bundle exec rake db:create
exit
```

