# Clair Server

Docker compose files and quick setup for running 
[clair](https://github.com/coreos/clair) on your local machine

Due to timing issues, start the postgres container and then the clair server
```bash
docker-compose up -d postgres
docker-compose up -d clair
```

The postgres data will be stored on your local directory under `postgres_data`
to speed up the re-build of the environment and persist analysis.

To shutdown execute
```bash
docker-compose stop
```
