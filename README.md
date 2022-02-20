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
| Bulb (B22)        | Athom      | LB01-7W-E27     | 1     | WLED               |
| Bulb (A19)        | Ikea       | LED1624G9       | 1     | Zigbee2MQTT        |
| **Entertainment**                                                             |
| Audio             | Chromecast | Audio           | 1     | HA :: Chromecast   |
| Speaker           | Sonos      | Play:5          | 1     | HA :: Sonos        |
| Receiver          | Yamaha     | HTR-8063        | 1     | HA :: MediaPlayers |
| Speaker           | Sonos      | Beam            | 1     | HA :: Sonos        |
| TV                | LG         | OLED55B8        | 1     | HA :: WebOSTV      |
| **Sensors**                                                                   |
| Air Quality       | PurpleAir  | PA-II           | 1     | RESP API           |
| Climate           | Ecobee     | v1              | 3     | HA :: Ecobee       |
| Climate           | Xiaomi     | WSDCGQ11LM      | 11    | Zigbee2MQTT        |
| Climate           | Xiaomi Mi  | LYWSD03MMC      | 3     | MQTT :: BLE Bridge |
| Contact           | Xiaomi     | MCCGQ11LM       | 15    | Zigbee2MQTT        |
| Leak              | Xiaomi     | SJCGQ11LM       | 11    | Zigbee2MQTT        |
| Motion            | Ikea       | E1745           | 1     | Zigbee2MQTT        |
| Motion            | Xiaomi     | RTCGQ11LM       | 3     | Zigbee2MQTT        |
| Plant             | Xiaomi     | Mi Flora (HHCC) | 2     | HA :: Mi Flora     |
| Temperature       | Acurite    | 592TXR          | 1     | MQTT :: rtl_433    |
| Temperature       | La Crosse  | TX141Bv3        | 4     | MQTT :: rtl_433    |
| Temperature       | La Crosse  | TX29IT          | 1     | MQTT :: rtl_433    |
| Vibration         | Xiaomi     | DJT11LM         | 1     | Zigbee2MQTT        |
| **Switches**                                                                  |
| Plug              | Gosund     | WP2             | 2     | Tasmota            |
| Plug              | Gosund     | WP5             | 3     | Tasmota            |
| Plug              | Sonoff     | S31             | 8     | Tasmota            |
| Plug              | Sonoff     | S31ZB           | 3     | Zigbee2MQTT        |
| Plug              | Wyze       | WLPPO1          | 1     | Tasmota            |
| Remote            | Ikea       | E1810           | 1     | Zigbee2MQTT        |
| Remote            | Xiaomi     | WXKG11LM        | 1     | Zigbee2MQTT        |
| Switch            | Shelly     | Plus 1PM        | 1     | Tasmota            |
| Switch            | Sonoff     | Mini R1         | 3     | Tasmota            |
| Switch            | Sonoff     | SV              | 1     | Tasmota            |
| Switch            | Treatlife  | SS02S           | 10    | Tasmota            |
| Switch (3 Way)    | Treatlife  | SS02            | 2     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS02S           | 3     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS01C           | 2     | Tasmota            |

 ### Infrastructure

 | Model           | Count | Role                                                              |
 | :---            | :--:  | :---                                                              |
 | NodeMCU ESP32   | 1     | [Bluetooth Low Energy Tracker Hub](esphome/house-ble-bridge.yaml) |
 | NooElec RTL-SDR | 1     | SDR USB Adapter w/ Antenna                                        |
 | Odroid-N2+      | 1     | [Home Assistant Blue](https://www.home-assistant.io/blue/) Server | 
 | Raspberry Pi 4  | 1     | Secondary Zigbee2MQTT server *                                    |
 | Slaesh CC2652RB | 2     | [Zigbee Adapter ](https://slae.sh/projects/cc2652/)               |
 | TP-Link UB400   | 1     | Bluetooth USB Adapter                                             |

 \* *I was having some issues with Zigbee mesh stability when running the Sinopé thermostat
 alongside the Xiaomi devices. From my understanding this is because Xiaomi doesn't completely
 comply with the Zigbee standards. I've decided to seperate them onto different Zigbee2MQTT
 servers and this seems to have addressed the issue with my lager mesh. Important note, I
 am carefully running these networks on channels far away from one another.*
