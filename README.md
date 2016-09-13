alpine-activemq
==============
[Docker](https://www.docker.com/) image for running [ActiveMQ] (http://activemq.apache.org/). Based on [Alpine Linux](http://alpinelinux.org/). 

[Image on Docker Hub](https://hub.docker.com/r/njmittet/alpine-activemq/).

Usage
-----
Run ActiveMQ with default configuration:
~~~~
docker run -d -P njmittet/alpine-activemq
~~~~

Ports
-----
Ports exposed by the image:

    8161  Web Console
    1883  MQTT 
    5672  AMQP 
    61613 STOMP
    61614 WS  
    61616 JMS

