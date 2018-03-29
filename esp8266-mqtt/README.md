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
``` if (client.connect("ESP8266Client")) { 
    ...
```

