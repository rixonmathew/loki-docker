# loki-docker
To setup loki with docker for ingesting logs
From https://techno-tim.github.io/posts/grafana-loki/

Add the following block to docker configuration to get docker logs in loki

```json
"log-opts": {
    "loki-url": "http://localhost:3100/loki/api/v1/push",
    "loki-batch-size": "400"
}
```
