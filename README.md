# Deployment

### Environment Variables

```sh
$ export POSTGRES_PASSWORD=PASSWORD
$ export SECRET_KEY_BASE=LONG_HASH
```

### Start

```sh
# Start containers
$ docker-compose up -d --force-recreate

# Database initial setup
$ docker-compose run web rake db:setup

# See logs
$ docker-compose logs web

# Stop
$ docker-compose stop
```
