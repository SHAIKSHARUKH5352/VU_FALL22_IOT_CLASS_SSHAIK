## What is MQTT?

MQTT ( MQ Telemetry Transport ) is a lightweight, publish-subscribe, machine to machine network protocol for Message queue/Message queuing service. It is designed for connections with remote locations that have devices with resource constraints or limited network bandwidth

## What is MQTT Broker?

An MQTT broker is a central software entity in the MQTT architecture. It acts just like a real estate broker which first does background checks on the parties involved and then after making sure that the relevant rules are enforced, the broker initiates a transaction.

## Mosquitto

Mosquitto is a lightweight open source message broker.

## Installing
 Go to '''https://www.mosquitto.org/download/''' and download the mosquitto MQTT broker.
 
 For the lastest mosquitto servers you need to tweek the config files to allow for external access. You need to find the config file used by your server.
To listen on addresses other than localhost, you need to have a config file with 
a "listener" line plus some authentication option. At its most wide-open, 
you could have:

listener 1883

allow_anonymous true

## ESP32 - Arduino IDE -  MQTT Code 

For publishing an MQTT message on topic esp32/dht/temperature

    uint16_t packetIdPub1 = mqttClient.publish(MQTT_PUB_TEMP, 1, true, String(temp).c_str());       
    
 For  publishg an MQTT message on topic esp32/dht/humidity
    uint16_t packetIdPub2 = mqttClient.publish(MQTT_PUB_HUM, 1, true, String(hum).c_str());        
    
    



