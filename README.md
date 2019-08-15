# arduino-mqtt-firebase
A project thar interfaces between arduino, mqtt and Firebase Realtime Database

# Summary
This project employs the concept of Wireless Sensor Networks to provide  real information from sensors  deployed in parking  slots. Components and Services used include:
* ESP-8266
* Firebase Realtime DB
* MQTT (HiveMQ) 

## MQTT

For the project, the NodeMCU was used to access MQTT services through an MQTT broker. NodeMCU gets distance from ultrasonic sensor. The ESP8266 Wi-Fi module connected to NodeMCU sends this distance to the internet. i.e., An MQTT client is associated with the Wi-Fi module sends the data to the specified MQTT server. The Wi-Fi module is integrated with the TCP/IP stack, and therefore MQTT protocol can be implemented with the help of Ponte Bridge,which is a multi-transport Internet of Things/M2M to Machine broker.
We chose `Hive MQ broker`, whose MQTT dashboard can be accessed via: https:// broker.mqtt-dashboard.com, where all incoming and outgoing messages through all channels in the broker can be seen. 

## Firebase

We implemented a  database  structure  using  Firebase, whose  main  advantage  is Database. Firebase  is a mobile and  web application development platform its Realtime that provides developers a variety  of tools and a  scalable  infrastructure  to build high quality  ap ps features: Realtime  Database and Cloud Functions The  Firebase  Realtime  Database  is a  cloud(&  Storage). We  utilized two of  its hosted  NoSQL  database  that sync  between our hardware sensor data and  application in realtime. This enabled us to the  Fire store  and base  database provide d our app with both the  current value of  the  data and  any  updates to  that data.
