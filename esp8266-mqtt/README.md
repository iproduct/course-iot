# Course Internet of Things (IoT)
Internet of Things (IoT) demos and examples with ESP8266 WiFi module 

## Arduino ESP8266 MQTT Client Demo
Demo shows how to implement bidirectional communication using MQTT protocol using ESP8266 WiFi module.

In order to run the demo you have to have running Messaaging Queus (MQ) Server.
You have to provide following settings to run the demo:

* ssid = "Your WiFi SSID";
* password = "Your WiFi password";
* mqtt_server = "Your MQTT Server IP address";
* mqtt_user = "Your MQTT Server username";
* mqtt_password = "Your MQTT Server password";

If you use anonimous MQTT connection (if you server allows it), you can skip specifing MQQT Server username and password, and you can change line 100 in the program to:
``` 
if (client.connect("ESP8266Client")) { 
    ...
```

## Installing Configuring and Running RabbitMQ Server
RabbitMQ is one of most widely used MQ server implementations. It is written in Erlang and provides outstanding performance and scalability as well as rich functionality on  a modular basis. In order to run it with the ESP8266 client you have to install it, enable MQTT module, and create a user for the demo.

### Installing RabbitMQ
1. JDK 8 - http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
2. OTP 20.3 full - http://www.erlang.org/downloads
3. RabbitMQ - http://www.rabbitmq.com/download.html
4. (Optional) NodeJS 9.x.x (latest)  - https://nodejs.org/en/download/current/

### Configuring RabbitMQ
 