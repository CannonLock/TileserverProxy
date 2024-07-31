Proxy requests to domain with added bearer header

Update the env variables according to the docker compose file and run the following command to start the server:

```shell
docker compose up
```

## Building

```shell
docker build --platform linux/amd64 -t hub.opensciencegrid.org/macrostrat/api-proxy:latest .
```

```shell
docker push hub.opensciencegrid.org/macrostrat/api-proxy:latest
```

## Running

```shell
docker run -p 8080:80 --env-file .env hub.opensciencegrid.org/macrostrat/api-proxy:latest
```