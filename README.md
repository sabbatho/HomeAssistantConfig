<p align="center">
  <img src="https://github.com/home-assistant/home-assistant-assets/blob/master/loading-screen.gif">
</p>

# Welcome! :)
I bought my first PI and started with [Home Assistant](https://home-assistant.io/) around the 25th of october 2018, using Telldus and z-wave.
Last of january 2019 i bought Raspbee and started tinkering with zigbee, changing to conbee around 25th of march 2019 to prepare for changing to a NUC or similar. I find the PI working ok, it's slow though and the SD might be the reason for strange restarts and having to restart now and then. So in the near future i will be changing to something more long term.
So yeah, having an SD-card crash i instantly went to buy an NUC and have used it since 27th of august 2019. Installed Ubuntu server and Docker on the NUC to finally install hassio. Works pretty good :) I'm not very used to Linux so some trial and error.
Must add that i am sad i didn't change from my PI earlier, crazy how much faster the NUC is.
And now at 2020-08-13 there has been no errors what so ever with the NUC. Super happy i changed!

So these are most of the [Home Assistant](https://home-assistant.io/) configuration files that i use. I am not in any shape or form educated to do programming. My primary use for HA is automation, my aim is to not be forced to press buttons or touch screens. Instead rules and automations should be smart enough to do what i want, of course with what i have. So no fancy frontend, just the most used and for fault searching.

For me this is alot of fun and to learn writing code.
I have searched around in others repos and communitys so i feel it's only fair that i give back what i can. :)


# Hardware:
* __[Intel NUC 8 i3](https://www.intel.com/content/www/us/en/products/boards-kits/nuc.html)__  - 256Gb SSD and 16Gb of ram, i know the ram is overkill for Home Assistant but since i am using Docker i have plans to expand for this NUC to do more.
* __[ConBee](https://phoscon.de/en/conbee)__ - Zigbee
* __[Aeon Labs Z-stick Gen5 USB-adapter](https://aeotec.com/z-wave-usb-stick)__ - Z-wave
* __[Logitech harmony Hub](https://www.logitech.com/en-gb/product/harmony-hub)__
* __[Fibaro universal sensor](https://www.fibaro.com/en/products/universal-binary-sensor/)__
* __[Lametric TIME](https://lametric.com/en-US/time/overview)__
* __[Chromecast ultra](https://store.google.com/product/chromecast_ultra)__ - had to be this one since the others won't stream 1080p 60hz
* __[Synology NAS, one of the older ones](https://www.synology.com/)__
* __[Telldus plugin z-wave switch](https://telldus.com/produkt/remote-controlled-outlet-telldus-z-wave/)__ - most used in my home
* __[Telldus z-wave plugin switch](https://telldus.com/produkt/plugin-receiver-mini-z-wave/)__ - have a few left, most have broken
* __[Osram smart+ E27 color](https://smartplus.ledvance.com/products/indoor-lighting/index.jsp)__ - pretty good colors, used to show outside temperature
* __[Osram smart+ E27 tunable](https://smartplus.ledvance.com/products/indoor-lighting/index.jsp)__ - Used with motion sensor
* __[Osram smart+ E14 candle tunable](https://smartplus.ledvance.com/products/indoor-lighting/index.jsp)__ - window lights, turning on with sun sensor
* __[Trust E27 color](https://www.trust.com/en/product/71145-zigbee-rgb-tunable-led-bulb-zled-rgb9)__ - not very good with colors, used as regular white lamp because of the colors not being so good
* __[Ikea trådfri E14 LED1649C5](https://www.ikea.com/gb/en/products/lighting/smart-lighting/tr%C3%A5dfri-led-bulb-e14-400-lumen-wireless-dimmable-warm-white-chandelier-opal-white-art-60365271/)__ - Works with ConBee but not Raspbee for me
* __[Philips HUE motion sensor](https://www2.meethue.com/en-us/p/hue-motion-sensor/046677473389)__ - Triggers lights in hallway and auto off when no motion
* __[Sonoff Basic](https://sonoff.itead.cc/en/)__ - Tasmota flashed and MQTT configured
* __[Sonoff TH10](https://sonoff.itead.cc/en/)__ - Tasmota flashed and MQTT configured, with temperature sensor
* __[Aqara motion sensor](https://www.aqara.com/en/human_motion_sensor.html)__ - Triggers lights in rooms

# Software windows clients
* __[Switch OFF](http://www.airytec.com/en/)__ - remote shutdown windows computers
* __[Plex](https://www.plex.tv/)__ - media stream software
* __[Putty](https://www.putty.org/)__ - SSH access, rarely used

# Software android clients
* __[Tasker](https://tasker.joaoapps.com/)__ - for battery info, charging status and incoming call notifications
* __[Overlook Whiz](https://apkpure.com/overlook-whiz/com.overlook.android.whiz)__ - Simple way to monitor my connection and external functions
* __[Pushbullet](https://www.pushbullet.com/)__ - Notifications
* __[Discord](https://discord.com/)__ - Notifications
* __[Home Assistant Companion](https://play.google.com/store/apps/details?id=io.homeassistant.companion.android/)__ - Notifications
* __[Owntracks](https://owntracks.org/)__ - for more advanced device tracking automations
* __[Simple RSS Widget](https://play.google.com/store/apps/details?id=de.j4velin.rssWidget&hl=en)__ - different status feeds

# Addons, components and special configs
* __[Duck DNS](https://www.home-assistant.io/addons/duckdns/)__ - Having trouble now and then with updates.
* __[Let's Encrypt](https://www.home-assistant.io/addons/duckdns/)__ - Using the one built in DuckDNS addon
* __[deCONZ](https://www.home-assistant.io/addons/deconz)__ - Zigbee controller
* __[Samba share](https://www.home-assistant.io/addons/samba/)__ - only started when i need it
* __[Google drive sync](https://github.com/sabeechen/hassio-google-drive-backup)__ - automated backup
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
* __[System health](https://www.home-assistant.io/components/system_health/)__ - For about page
* __[Command line sensor](https://www.home-assistant.io/components/sensor.command_line/)__ - tracking current version and installed version for pushbullet notifications
* __[File size sensor](https://www.home-assistant.io/components/sensor.filesize/)__ - tracking file size of .log, mostly used it when i was troubleshooting problems i had
* __[Shell commands](https://www.home-assistant.io/components/shell_command/)__ - used for communicating with lametric and swtich off software. A few ugly bash scripts for the lamteric stuff
* __[Shoppinglist](https://www.home-assistant.io/components/shopping_list/)__ - What am i gonna buy?
* __[Workday](https://www.home-assistant.io/components/workday/)__ - used for wakeup automations on workdays only
* __[Mosquitto MQTT broker](https://www.home-assistant.io/addons/mosquitto/)__ - At the moment for Sonoff devices only
* __[MQTT](https://www.home-assistant.io/components/mqtt/)__ - At the moment for Sonoff devices only
* __[TasmoAdmin](https://github.com/hassio-addons/addon-tasmoadmin)__ - Manage Tasmota devices
* __[Visual Studio Code](https://github.com/hassio-addons/addon-vscode)__ - Editing installation
* __[Wireguard](https://github.com/hassio-addons/addon-wireguard)__ - VPN
* __[Chrony](https://github.com/hassio-addons/addon-chrony)__ - Server time management




# More to come in this file! I have atleast started it :)
