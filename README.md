# ESP8266-AlexaSwitch
Smart switch to control almost anything using Alexa with voice commands. 

## Hardware used
1. ESP-8266 Development Board (NodeMCU)
2. 4-Channel 5V Relay Board
3. Mini Breadboard
4. Dupont wires
5. Amazon Echo Dot

## Softwares
1. Arduino IDE (To upload code to NodeMCU Board)

## Instructions

### Upload arduino sketch to NodeMCU
1. Download and install WebSocketsClient.h and ArduinoJson.h libraries
   WebSocketsClient.h :https://github.com/kakopappa/sinric/wiki/How-to-add-dependency-libraries
   ArduinoJson.h      :https://github.com/kakopappa/sinric/wiki/How-to-add-dependency-libraries
2. Open Arduino IDE and select Board Manager
   Tools > Board > Boards Manager. Install ESP8266
3. Select board NodeMCU 1.0(ESP-12E Module)
4. Download the sketch ESP-8266_Alexa_Switch.ino and upload

### Using Alexa to control NodeMCU
1. Register for an account on sinric (https://sinric.com) 
2. Login and create smart home devices (Dashboard -> Add smart home device)
3. Copy the API Key generated from dashboard
4. Connect to Sinric server - Use ESP-8266_Alexa_Switch.ino sketch
5. In the Arduino Sketch ESP-8266_Alexa_Switch.ino Replace the API Key, Wifi SSID and Password copied from sinric
6. Change the Device IDs in ESP-8266_Alexa_Switch.ino Code to that supplied on Sinric website for each device
7. In Amazon Alexa app enable sinric skill and link to your sinric account.
8. From the Alexa app (Devices tab) add/discover new devices, you will see the new device names as mentioned in the arduino sketch.
9. Start using by saying "Alexa, turn on "device name", "Alexa, turn off "device name"

## Credits
Aruna Tennakoon - https://github.com/kakopappa
