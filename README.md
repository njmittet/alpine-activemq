alpine-activemq
===============
[Docker](https://www.docker.com/) image for running [ActiveMQ](http://activemq.apache.org/). Based on [Alpine Linux](http://alpinelinux.org/). 

[Image on Docker Hub](https://hub.docker.com/r/trifonnt/alpine-activemq/).


How to build Docker image
-------------------------
```shell
docker build -t trifonnt/alpine-activemq:5.15.2 .
```

How to push to Docker hub
-------------------------
```shell
docker push trifonnt/alpine-activemq:5.15.2
```

Usage
-----
Run ActiveMQ with default configuration:
```shell
docker run --name my-activemq-5.15.2 -d -P -p 8161:8161 -p 1883:1883 -p 5672:5672 -p 61613:61613 -p 61614:61614 -p 61616:61616 trifonnt/alpine-activemq:5.15.2
```

Ports
-----
Ports exposed by the image:

    8161  Web Console
    1883  MQTT
    5672  AMQP
    61613 STOMP
    61614 WS
    61616 JMS

Application URLs
----------------
admin/admin
[http://localhost:8161/](http://localhost:8161/)


Links
-----
 - https://github.com/mbogner/docker-activemq

 - https://hub.docker.com/r/webcenter/activemq/
