## About

This is my personal Home Assistant configuration. My guiding principle is to have
full local control of all my devices. Below you will find a table of all the devices
in my house that are integrated into home assistant. i've captured a bit about how
they're connected.

You will notice there are frequent updates here, so please feel free to follow along.
And, if you have any feedback, please feel free to reach out :smile:

### Devices

| Type              | Make       | Model           | Count | Connectivity       |
| :---              | :---       | :---            | :--:  | :--                |
| **HVAC**                                                                      |
| Thermostat        | Ecobee     | Ecobee3         | 1     | HA :: Ecobee       |
| Thermostat        | Sinopé     | TH1400ZB        | 1     | Zigbee2MQTT        |
| **Lights**                                                                    |
| Bulb (A25)        | Athom      | LB01-15W-E27    | 2     | Tasmota            |
| Bulb (BR30)       | Athom      | LB03-12W-BR30   | 2     | Tasmota            |
| Bulb (A19)        | Ikea       | LED1624G9       | 1     | Zigbee2MQTT        |
| **Entertainment**                                                             |
| Audio             | Chromecast | Audio           | 1     | HA :: Chromecast   |
| Speaker           | Sonos      | Play:5          | 1     | HA :: Sonos        |
| Receiver          | Yamaha     | HTR-8063        | 1     | HA :: MediaPlayers |
| Speaker           | Sonos      | Beam            | 1     | HA :: Sonos        |
| TV                | LG         | OLED55B8        | 1     | HA :: WebOSTV      |
| **Sensors**                                                                   |
| Air Quality       | PurpleAir  | PA-II           | 1     | RESP API           |
| Climate           | SensorPush | HT1             | 4     | HACS :: SensorPush |
| Climate           | Ecobee     | v1              | 3     | HA :: Ecobee       |
| Climate           | Tuya       | TS0201          | 1     | Zigbee2MQTT        |
| Climate           | Xiaomi     | WSDCGQ11LM      | 12    | Zigbee2MQTT        |
| Contact           | Xiaomi     | MCCGQ11LM       | 15    | Zigbee2MQTT        |
| Leak              | Xiaomi     | SJCGQ11LM       | 10    | Zigbee2MQTT        |
| Motion            | Ikea       | E1745           | 1     | Zigbee2MQTT        |
| Motion            | Xiaomi     | RTCGQ11LM       | 3     | Zigbee2MQTT        |
| Plant             | Xiaomi     | Mi Flora (HHCC) | 2     | HA :: Mi Flora     |
| Vibration         | Xiaomi     | DJT11LM         | 1     | Zigbee2MQTT        |
| **Switches**                                                                  |
| Plug              | Gosund     | WP2             | 2     | Tasmota            |
| Plug              | Gosund     | WP5             | 3     | Tasmota            |
| Plug              | Sonoff     | S31             | 4     | Tasmota            |
| Plug              | Sonoff     | S31ZB           | 3     | Zigbee2MQTT        |
| Remote            | Ikea       | E1810           | 1     | Zigbee2MQTT        |
| Switch            | Sonoff     | Mini R1         | 3     | Tasmota            |
| Switch            | Sonoff     | SV              | 1     | Tasmota            |
| Switch            | Treatlife  | SS02S           | 10    | Tasmota            |
| Switch (3 Way)    | Treatlife  | SS02            | 2     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS02S           | 3     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS01C           | 2     | Tasmota            |

 ### Infrastructure

 | Model           | Role                                                              |
 | :---            | :---                                                              |
 | Odroid-N2+      | [Home Assistant Blue](https://www.home-assistant.io/blue/) Server | 
 | Slaesh CC2652RB | [Zigbee Adapter ](https://slae.sh/projects/cc2652/)               |
 | TP-Link UB400   | Bluetooth USB Adapter                                             |