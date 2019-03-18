<p align="center">
  <img src="https://github.com/home-assistant/home-assistant-assets/blob/master/loading-screen.gif">
</p>

# Welcome! :)
These are most of the [Home Assistant](https://home-assistant.io/) configuration files that i use. I am not in any shape or form educated to do programming. My primary use for HA is automation, my aim is to not be forced to press buttons or touch screens. Instead rules and automations should be smart enough to do what i want, of course with what i have. So no fancy frontend, just the most used and for fault searching.
For me this is alot of fun and to learn writing code.
I have searched around in others repos and communitys so i feel it's only fair that i give back what i can. :)

# Hardware:
* __[Raspberry Pi3 Model B+](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/)__  - with SDcard 16GB class 10
* __[Raspbee](https://www.dresden-elektronik.de/funktechnik/products/boards-and-kits/development-boards/raspbee/)__
* __[Aeon Labs Z-stick Gen5 USB-adapter](https://aeotec.com/z-wave-usb-stick)__
* TellStick.NET (to be removed from setup)
* TellStick ZNet Lite v2 (to be removed from setup)
* __[Logitech harmony Hub](https://www.logitech.com/en-gb/product/harmony-hub)__
* __[Fibaro universal sensor](https://www.fibaro.com/en/products/universal-binary-sensor/)__
* __[Lametric TIME](https://lametric.com/en-US/time/overview)__
* __[Chromecast 2nd gen](https://store.google.com/product/chromecast)__
* __[Synology NAS, one of the older ones](https://www.synology.com/)__
* __[Telldus plugin z-wave switch](https://telldus.com/produkt/remote-controlled-outlet-telldus-z-wave/)__ - most used in my home
* __[Telldus z-wave plugin switch](https://telldus.com/produkt/plugin-receiver-mini-z-wave/)__ - have a few left, most have broken
* __[Osram smart+ E27 color](https://smartplus.ledvance.com/products/indoor-lighting/index.jsp)__ - pretty good colors, used to show outside temperature
* __[Trust E27 color](https://www.trust.com/en/product/71145-zigbee-rgb-tunable-led-bulb-zled-rgb9)__ - not very good with colors, used as regular white lamp because of the colors not being so good
* __[Ikea trådfri E14 LED1649C5](https://www.ikea.com/gb/en/products/lighting/smart-lighting/tr%C3%A5dfri-led-bulb-e14-400-lumen-wireless-dimmable-warm-white-chandelier-opal-white-art-60365271/)__ - Still trying to connect, not working for mer yet, sad face

# Software windows clients
* __[Switch OFF](http://www.airytec.com/en/)__ - remote shutdown windows computers
* __[Plex](https://www.plex.tv/)__ - media stream software
* __[Putty](https://www.putty.org/)__ - SSH access, rarely used

# Software android clients
* __[Tasker](https://tasker.joaoapps.com/)__ - for battery info, charging status and incoming call notifications
* __[Pushbullet](https://www.pushbullet.com/)__ - most important notifications
* __[HomeAssist](https://github.com/ascillato/HomeAssist-Android-App)__ - manual switching
* __[Owntracks](https://owntracks.org/)__ - for more advanced device tracking automations
* __[Simple RSS Widget](https://play.google.com/store/apps/details?id=de.j4velin.rssWidget&hl=en)__ - different status feeds

# Addons, components and special configs
* __[MariaDB](https://www.home-assistant.io/addons/mariadb/)__ - much more stable with MariaDB instead of standard SQLite
* __[Configurator](https://www.home-assistant.io/addons/configurator)__ - almost only use this for configuration
* __[Duck DNS](https://www.home-assistant.io/addons/duckdns/)__ - not much to say, LetsEncrypt also enabled
* __[deCONZ](https://www.home-assistant.io/addons/deconz)__ - Zigbee controller
* __[Samba share](https://www.home-assistant.io/addons/samba/)__ - only started when i need it
* __[SSH server](https://www.home-assistant.io/addons/ssh/)__ - only started when i need it
* __[Dropbox Sync](https://github.com/danielwelch/hassio-dropbox-sync)__ - automated backup
* __[Telldus Live](https://www.home-assistant.io/components/tellduslive/)__ - to be removed, way to unstable for my taste
* __[SMHI](https://www.home-assistant.io/components/smhi/)__ - sending data to the lametric
* __[YR](https://www.home-assistant.io/components/sensor.yr/)__ - sending data to the lametric
* __[Owntracks](https://www.home-assistant.io/components/owntracks/)__ - device tracking
* __[NMAP](https://www.home-assistant.io/components/device_tracker.nmap_tracker/)__ - device tracking
* __[Z-wave](https://www.home-assistant.io/components/zwave/)__ - Z-wave controller
* __[Google Cast](https://www.home-assistant.io/components/cast/)__ - controlling and "what's playing"
* __[Wake on lan](https://www.home-assistant.io/components/wake_on_lan/)__ - start computers
* __[Media player Plex](https://www.home-assistant.io/components/media_player.plex/)__ - "what's playing" to lametric
* __[Media extractor](https://www.home-assistant.io/components/media_extractor/)__ - automated youtube play to chromecast
* __[Pushbullet](https://www.home-assistant.io/components/notify.pushbullet/)__ - automated notifications like new version or unwanted restarts
* __[RSS feed template](https://www.home-assistant.io/components/rss_feed_template/)__ - for android widget
* __[Notify file](https://www.home-assistant.io/components/notify.file/)__ - sensor data to lametric
* __[Sun](https://www.home-assistant.io/components/sun/)__ - used for automations
* __[Date and time sensor](https://www.home-assistant.io/components/sensor.time_date/)__ - used for specific automations, example x-mas lights
* __[Uptime](https://www.home-assistant.io/components/sensor.uptime/)__ - tracking for pushbullet notifications
* __[Synology DSM](https://www.home-assistant.io/components/sensor.synologydsm/)__ - tracking disc free
* __[Trafikverket](https://www.home-assistant.io/components/sensor.trafikverket_weatherstation/)__ - tracking temprature and precipitation
* __[System monitor](https://www.home-assistant.io/components/sensor.systemmonitor/)__ - tracking disc free on SDcard
* __[Command line sensor](https://www.home-assistant.io/components/sensor.command_line/)__ - tracking current version and installed version for pushbullet notifications
* __[File size sensor](https://www.home-assistant.io/components/sensor.filesize/)__ - tracking file size of .log, mostly used it when i was troubleshooting problems i had
* __[Shell commands](https://www.home-assistant.io/components/shell_command/)__ - used for communicating with lametric and swtich off software. A few ugly bash scripts for the lamteric stuff





# More to come in this file! I have atleast started it :)
