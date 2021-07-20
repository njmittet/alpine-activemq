# alpine-activemq

A [Docker](https://www.docker.com/) image for running [ActiveMQ](http://activemq.apache.org/). Based on
[njmittet/alpine-adoptopenjdk:16-jre-hotspot](https://hub.docker.com/repository/docker/njmittet/alpine-adoptopenjdk).

[Image on Docker Hub](https://hub.docker.com/repository/docker/njmittet/alpine-activemq).

## Usage

Pull the image from Docker Hub:

```SH
docker pull njmittet/alpine-activemq:5.16.2
```

Run ActiveMQ with default configuration:

```SH
docker run -d -P njmittet/alpine-activemq:5.16.2
```

## Ports

Ports exposed by the image:

```SH
8161  Web Console
1883  MQTT
5672  AMQP
61613 STOMP
61614 WS
61616 JMS
```
