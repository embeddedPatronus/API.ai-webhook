# Description
Webhook for interacting with google's api.ai and sending the interaction payload to MQTT broker


A nodejs script that connects with api.ai and takes the speech payload and send it to HiveMQ MQTT broker.It lets your IoT devices
interact with google's ai engine such as api.ai.

# Pre-requisites

1. IoT device subscribed to HiveMQ broker on the topics given in the nodejs script.
2. Configuring api.ai so that it sends a post request to the nodejs script.

# How it works
When the user say something, api.ai recognizes the speech and take the necessary action by sending the speech intent to the post 
server listening on the port 5000.
The payload is then sent to the MQTT HiveMQ broker so that it may be available to all the MQTT clients connected to it.
A user can set up an IoT device running an HiveMQ MQTT client and subscibed to the same topic.Now the user can receive the speech's
intent and take the necessary actions. 

It was primarily built for workplace automation and monitoring but one can pretty much do anything on this communication link.
Enjoy


# Author
Gaurav Sharma
LinkedIn - https://www.linkedin.com/in/gauravsharma49/
Gmail - gaurav.sharma0394@gmail.com

