# Minimal Spark Cluster for local development

If you are trying to spin up a small spark cluster for local development use this template to just deploy it with docker

# Installation

Images are built automatically when calling docker-compose 

`docker-compose up`

You might want to change the amount of CPUs and RAM in docker-compose.yaml

## Accessing the Spark Cluster

The master node is accessible via the IP you gave it, e.g.  
- http://10.5.0.2:8080/ in the Docker network, or
- localhost:9191 in the host 
