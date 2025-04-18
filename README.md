# homeassistant
Project contains some explanations how to setup and configure complex solutions with Home Assistant, ESPHome and self-ironed IOT devices.

# ESP32 + Screen ILI9488

Yaml config to show weather forecast on ESP32 + ILI9488 screen. 
The main idea is to display the weather forecast in graphical format on a color screen.

<img src="https://github.com/apih9000/homeassistant/blob/main/screenshots/ILI9488-1.jpeg?raw=true" width="160px" />

Look at the config yaml in the "esphome" folder. 

Hardware consist of 3 items: ESP32 S3 Wroom 1 N16R8 + ILI9488 screen + PIR sensor. 
PIR sensor is used to activate screen backlight when someone is in the room, and turn the screen off in case of innactivity in the room. 

The screen contains 4 main regions:
1) Air quality index – External data from https://waqi.info/ 
2) Current temperature – Realtime temperature from my own outside hardware temperature sensor.
3) Image of the weather prediction for today, and low-max temperature prediction for today – External weather prediction.
4) Current time.

<img src="https://github.com/apih9000/homeassistant/blob/main/screenshots/ILI9488-2.jpeg?raw=true" width="160px" />
