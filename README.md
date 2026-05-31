# iot-mqtt-command-system
This project demonstrates a real-time IoT command system using MQTT and Node-RED to remotely control a mobile device.  Commands are sent from Node-RED, passed through an MQTT broker, and executed on a mobile phone using Tasker and Termux.  The system is generic and can be extended beyond the demo use case (music control).


Architecture :
Node-RED (ZimaBoard)
        ↓
MQTT Broker (Proxmox - Mosquitto)
        ↓
Mobile Device (Tasker + Termux)
        ↓
Action Execution

Technologies:
Node-RED
Mosquitto MQTT Broker
Proxmox VE
ZimaBoard 832
Tasker (Android)
Termux
MQTT Explorer

MQTT Topics Example:
iot/mobile/command/play
iot/mobile/command/stop
iot/mobile/command/notify

Demo Use Case:
Music control is used only as a demonstration.
The system can be extended to:
- Notifications
- App control
- Smart home automation
- Remote command execution

Screenshots:
Node-RED flow
MQTT Explorer messages
Termux subscriber output

How it works:
1. Node-RED sends MQTT message  
2. MQTT broker receives it  
3. Mobile subscribes to topic  
4. Tasker/Termux executes action


This project is part of my IoT and embedded systems learning journey.

