# Kafka Monitor Kubernetes Docker build
How to build this image 
## Getting Started

### Build the container locally
Decide where you would like the built container to be stored.  The 
default is quay.io/samsung_cnct/kafka-monitor.  You can probably not
write to this location so you should update the Makefile with your
repository name.  

When complete execute
```
make container
```

### Push container to remote repository
```
make push
```
