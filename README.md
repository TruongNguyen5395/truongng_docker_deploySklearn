# flask-sklearn

Application to deploy sklearn models


## Build

```bash
docker build -t truongng/deploy-sklearn:latest .
```

## Run container

```bash
docker run \
    --name=deploy-sklearn \
    --rm \
    -v <path/to/model/on/host:/path/to/model/in/docker \
    -e MODEL_PATH=/path/to/model/in/docker \
    -p <port>:9000 \
        mlrepa/deploy-sklearn:latest
```

