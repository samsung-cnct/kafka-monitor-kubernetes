# kafka-monitor-kubernetes
create pod and service for kafka monitor

## Why
kafka-monitor provides a continuous test of the targeted kafka cluster's performance
along several metrics.  

## Bootstrap
Create the petset in this directory
```
kubectl create -f kafka-monitor.yaml
```

## Dependencies
Kafka-monitor requires a running kafka cluster and will enter a crash/backoff loop until the kafka cluster is running.  Ensure the kafka svc name in the .properties file matches your kafka cluster to monitor.

## Resources
node:
 - 500MB
 - 1/8 CPU (125m)