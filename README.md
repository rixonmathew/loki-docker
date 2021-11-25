# loki-docker
To setup loki with docker for ingesting logs

Add the following block to docker configuration to get docker logs in loki
"log-opts": {
    "loki-url": "http://localhost:3100/loki/api/v1/push",
        "loki-batch-size": "400"
          },
