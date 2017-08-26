alpine-activemq
===============
[Docker](https://www.docker.com/) image for running [ActiveMQ](http://activemq.apache.org/). Based on [Alpine Linux](http://alpinelinux.org/). 

[Image on Docker Hub](https://hub.docker.com/r/trifonnt/alpine-activemq/).


How to build Docker image
-------------------------
```shell
docker build -t trifonnt/alpine-activemq:5.15.0 .
```

How to push to Docker hub
-------------------------
```shell
docker push trifonnt/alpine-activemq:5.15.0
```

Usage
-----
Run ActiveMQ with default configuration:
```shell
docker run --name my-activemq -d -P -p 8161:8161 trifonnt/alpine-activemq:5.15.0
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
http://localhost:8161/


Links
-----
https://github.com/mbogner/docker-activemq
https://hub.docker.com/r/webcenter/activemq/
