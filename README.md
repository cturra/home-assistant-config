## About

This is my personal Home Assistant configuration. My guiding principle is to have
full local control of all my devices. Below you will find a table of all the devices
in my house that are integrated into home assistant. i've captured a bit about how
they're connected.

You will notice there are frequent updates here, so please feel free to follow along.
And, if you have any feedback, please feel free to reach out :smile:

### Devices

| Type              | Make       | Model           | Count | Connectivity          |
| :---              | :---       | :---            | :--:  | :--                   |
| **HVAC**                                                                         |
| Thermostat        | Ecobee     | Ecobee3         | 1     | HA :: Ecobee          |
| Thermostat        | Sinopé     | TH1400ZB        | 1     | Zigbee2MQTT           |
| **Lights**                                                                       |
| Bulb (A25)        | Athom      | LB01-15W-E27    | 1     | Tasmota               |
| Bulb (BR30)       | Philips    | 046677577957    | 2     | Zigbee2MQTT           |
| Bulb (E26)        | Philips    | 9290024687      | 1     | Zigbee2MQTT           |
| Bulb (E26)        | Philips    | 929002478401    | 1     | Zigbee2MQTT           |
| Bulb (E26)        | Philips    | 9290024717      | 2     | Zigbee2MQTT           |
| Floor Lamp        | Govee      | H6076           | 1     | HA :: Govee           |
| **Locks**                                                                        |
| Door Lock         | August     | ASL-03          | 2     | HA :: Yale Access BLE |
| **Entertainment**                                                                |
| Audio             | Chromecast | Audio           | 1     | HA :: Chromecast      |
| Receiver          | Yamaha     | HTR-8063        | 1     | HA :: MediaPlayers    |
| Speaker           | Sonos      | Beam            | 1     | HA :: Sonos           |
| Speaker           | Sonos      | Play:5          | 1     | HA :: Sonos           |
| Speaker           | Sonos      | Roam SL         | 1     | HA :: Sonos           |
| TV                | LG         | OLED55B8        | 1     | HA :: WebOSTV         |
| TV                | LG         | OLED65C1        | 1     | HA :: WebOSTV         |
| **Sensors**                                                                      |
| Air Quality       | Awair      | Element         | 3     | HA :: Awair Local API |
| Air Quality       | Airthings  | Wave+           | 1     | HA :: Airthings BLE   |
| Air Quality       | PurpleAir  | PA-II           | 1     | RESP API              |
| BLE Proxy         | M5Stack    | ATOM Lite       | 6     | ESPHome               |
| Climate           | Ecobee     | v1              | 3     | HA :: Ecobee          |
| Climate           | Inkbird    | IBS-TH2         | 3     | HA :: Inkbird BLE     |
| Climate           | Xiaomi     | WSDCGQ11LM      | 1     | Zigbee2MQTT           |
| Climate           | Xiaomi Mi  | LYWSD03MMC      | 8     | HA :: BTHome          |
| Contact           | Ikea       | E2013           | 4     | Zigbee2MQTT           |
| Contact           | Xiaomi     | MCCGQ11LM       | 14    | Zigbee2MQTT           |
| Leak              | Ikea       | E2202           | 2     | Zigbee2MQTT           |
| Leak              | Xiaomi     | SJCGQ11LM       | 15    | Zigbee2MQTT           |
| Motion            | Ikea       | E1745           | 1     | Zigbee2MQTT           |
| Motion            | Ikea       | E2134           | 1     | Zigbee2MQTT           |
| Motion            | Philips    | 9290030674      | 2     | Zigbee2MQTT           |
| Motion            | Xiaomi     | RTCGQ14LM       | 1     | Zigbee2MQTT           |
| Presence          | Tuya       | ZY-M100         | 2     | ESPHome               |
| Plant             | Xiaomi     | Mi Flora (HHCC) | 3     | HA:: Xiami BLE        |
| Smoke             | Nest       | Protect         | 4     | HACS :: Nest Proect   | 
| Temperature       | Acurite    | 592TXR          | 3     | MQTT :: rtl_433       |
| Temperature       | La Crosse  | TX141Bv3        | 4     | MQTT :: rtl_433       |
| Vibration         | Xiaomi     | DJT11LM         | 1     | Zigbee2MQTT           |
| **Surveillance**                                                                 |
| Camera            | ACTi       | B87             | 1     | RTSP                  |
| Camera Doorbell   | Amcrest    | AD410           | 1     | HACS :: Dahua         |
| Camera            | Reolink    | E1 Pro          | 1     | RTSP                  |
| Camera            | Meraki     | MV72            | 1     | RTSP                  |
| Camera            | Wyze       | Cam v3          | 1     | RTSP                  |
| **Switches**                                                                     |
| IR Blaster        | Uniplay    | Q1              | 3     | Tasmota               |
| Plug              | Gosund     | WP2             | 2     | Tasmota               |
| Plug              | Gosund     | WP5             | 3     | Tasmota               |
| Plug              | Sonoff     | S31             | 8     | Tasmota               |
| Plug              | Sonoff     | S31ZB           | 3     | Zigbee2MQTT           |
| Plug              | Wyze       | WLPPO1          | 1     | Tasmota               |
| Receptacle        | TopGreener | TGWF15RM        | 1     | Tasmota               |
| Remote            | Ikea       | E1810           | 2     | Zigbee2MQTT           |
| Remote            | Ikea       | E2123           | 3     | Zigbee2MQTT           |
| Remote            | Xiaomi     | WXKG11LM        | 1     | Zigbee2MQTT           |
| Switch (Motion)   | CloudFree  | SWM1            | 1     | Tasmota               |
| Switch (Motion)   | Milfra     | MFA06           | 1     | Tasmota               |
| Switch            | Shelly     | 1               | 1     | Tasmota               |
| Switch (Energy)   | Shelly     | EM              | 1     | Tasmota               |
| Switch (USB)      | Sinilink   | XY-WFUSB        | 1     | Tasmota               |
| Switch            | Sonoff     | Basic           | 1     | Tasmota               |
| Switch            | Sonoff     | Mini R1         | 2     | Tasmota               |
| Switch            | Sonoff     | SV              | 1     | Tasmota               |
| Switch            | Treatlife  | SS02S           | 12    | Tasmota               |
| Switch (3 Way)    | Treatlife  | SS02            | 2     | Tasmota               |
| Switch (Dimmer)   | Treatlife  | DS02S           | 4     | Tasmota               |
| Switch (Dimmer)   | Treatlife  | DS01C           | 3     | Tasmota               |
| **Other**                                                                        |
| Air Purifier      | Dyson      | TP02            | 1     | HACS :: Dyson         |
| Air Purifier      | Dyson      | BP01            | 2     | infrared              |
| Air Purifier      | Dyson      | HP07            | 1     | HACS :: Dyson         |
| Propane Tank      | Mopeka     | Pro Check M1017 | 1     | HA :: Mopeka          |
| Toothbrush        | Oral-B     | Smart 4000      | 2     | HA :: Oral-B          |

 ### Infrastructure

 | Model           | Count | Role                                                              |
 | :---            | :--:  | :---                                                              |
 | RTL-SDR         | 2     | SDR USB Adapters w/ Antenna                                       |
 | Odroid-N2+      | 1     | [Home Assistant Blue](https://www.home-assistant.io/blue/) Server | 
 | Raspberry Pi 4  | 1     | Secondary Zigbee2MQTT server *                                    |
 | Slaesh CC2652RB | 2     | [Zigbee Adapter ](https://slae.sh/projects/cc2652/)               |
 | ASUS BT500      | 1     | Bluetooth USB Adapter                                             |

 \* *I was having some issues with Zigbee mesh stability when running the Sinopé thermostat
 alongside the Xiaomi devices. From my understanding this is because Xiaomi doesn't completely
 comply with the Zigbee standards. I've decided to seperate them onto different Zigbee networks
 and this seems to have addressed the issue with my larger mesh. Important note, I
 am carefully running these networks on channels far away from one another.*
