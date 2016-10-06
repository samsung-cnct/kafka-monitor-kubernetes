FROM quay.io/coffeepac/kafka-monitor:0.1

MAINTAINER coffeepac@gmail.com

WORKDIR /opt/kafka-monitor
ADD kafka-monitor.properties config/kafka-monitor.properties

# Use "exec" form so that it runs as PID 1 (useful for graceful shutdown)
CMD ["/opt/kafka-monitor/kafka-monitor-docker-entry.sh"]
