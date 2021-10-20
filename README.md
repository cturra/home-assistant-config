## About

This is my personal Home Assistant configuration. My guiding princile is to have
full local control of all my devices. I intend everything to run Tasmota, 
ESPHome or speak Zigbee to my MQTT broker.

This project still an active work in progress. Stay tuned for more information about
what hardware I am using, how it's configured, etc.

For now, please enjoy, and feedback always welcome!

| Type              | Make       | Model         | Count | Connectivity       |
| :---              | :---       | :---          | :--:  | :--                |
| **HVAC**          |
| Thermostat        | Ecobee     | Ecobee3       | 1     | HA :: Ecobee       |
| Thermostat        | Sinopé     | TH1400ZB      | 1     | Zigbee2MQTT        |
| **Lights**        |
| Bulb (A25)        | Athom      | LB01-15W-E27  | 2     | Tasmota            |
| Bulb (BR30)       | Athom      | LB03-12W-BR30 | 2     | Tasmota            |
| Bulb (A19)        | Ikea       | LED1624G9     | 1     | Zigbee2MQTT        |
| **Entertainment** |
| Audio             | Chromecast | Audio         | 1     | HA :: Chromecast   |
| Speaker           | Sonos      | Play:5        | 1     | HA :: Sonos        |
| Receiver          | Yamaha     | HTR-8063      | 1     | HA :: MediaPlayers |
| Speaker           | Sonos      | Beam          | 1     | HA :: Sonos        |
| TV                | LG         | OLED55B8      | 1     | HA :: WebOSTV      |
| **Sensors**       |
| Air Quality       | PurpleAir  | PA-II         | 1     | RESP API           |
| Climate           | SensorPush | HT1           | 4     | HACS :: SensorPush |
| Climate           | Ecobee     | v1            | 3     | HA :: Ecobee       |
| Climate           | Tuya       | TS0201        | 1     | Zigbee2MQTT        |
| Climate           | Xiaomi     | WSDCGQ11LM    | 11    | Zigbee2MQTT        |
| Contact           | Xiaomi     | MCCGQ11LM     | 15    | Zigbee2MQTT        |
| Leak              | Xiaomi     | SJCGQ11LM     | 10    | Zigbee2MQTT        |
| Motion            | Ikea       | E1745         | 1     | Zigbee2MQTT        |
| Motion            | Xiaomi     | RTCGQ11LM     | 3     | Zigbee2MQTT        |
| Vibration         | Xiaomi     | DJT11LM       | 1     | Zigbee2MQTT        |
| **Switches**      |
| Plug              | Gosund     | WP2           | 1     | Tasmota            |
| Plug              | Gosund     | WP5           | 3     | Tasmota            |
| Plug              | Sonoff     | S31           | 4     | Tasmota            |
| Plug              | Sonoff     | S31ZB         | 3     | Zigbee2MQTT        |
| Remote            | Ikea       | E1810         | 1     | Zigbee2MQTT        |
| Switch            | Sonoff     | Mini R1       | 3     | Tasmota            |
| Switch            | Sonoff     | SV            | 1     | Tasmota            |
| Switch            | Treatlife  | SS02S         | 9     | Tasmota            |
| Switch (3 Way)    | Treatlife  | SS02          | 2     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS02S         | 3     | Tasmota            |
| Switch (Dimmer)   | Treatlife  | DS01C         | 2     | Tasmota            |