# Home-Assistant-Configuration [![Build Status](https://travis-ci.org/stanvx/Home-Assistant-Configuration.svg?branch=master)](https://travis-ci.org/stanvx/Home-Assistant-Configuration)
[Home Assistant](https://home-assistant.io/) configuration files (YAMLs). These are my Home Assistant configuration files.
#### Navigation:
* Home Assistant Configuration files are now mostly located within [Packages directory](https://github.com/stanvx/Home-Assistant-Configuration/tree/master/packages).
* AppDaemon Dashboard Configuration files can be found within the [AppDaemon directory](https://github.com/stanvx/Home-Assistant-Configuration/tree/master/appdaemon/dashboards).
* HA Floorplan Configuration files including my SVG file can be found within the [www/customui/floorplan directory](https://github.com/stanvx/Home-Assistant-Configuration/tree/master/www/custom_ui/floorplan)

# Devices
* [Intel NUC8I7BEH](https://www.intel.com.au/content/www/au/en/products/boards-kits/nuc/kits/nuc8i7beh.html) - Ubuntu Server 18.04 with Hass.io.
* [Aeotec Z-Stick Gen5](http://aeotec.com/z-wave-usb-stick)
* [Synology DSM1815+ 8 Bay NAS](https://www.synology.com/en-global/products/DS1817+)
* [CyberPower CP1300EPFCLCD UPS](https://www.cyberpower.com/vn/en/product/sku/CP1300EPFCLCD)
* [Reolink RLC-422-P IP Camera](https://reolink.com/product/rlc-422/) x2
* [Lenovo Tab 4, 8" Android Tablet](https://www3.lenovo.com/au/en/tablets-and-2-in-1s/android-tablets/Lenovo-TB-8504/p/ZZITZTATB08) - Used with [HADashboard](https://play.google.com/store/apps/details?id=de.ozerov.fully) and [MQTT Alarm Control Panel](https://play.google.com/store/apps/details?id=com.thanksmister.iot.mqtt.alarmpanel)
* [KAS Z-Wave Door Lock](https://kas.com.au/online-store/z-wavedoorlock/)
* [Xiaomi Roborock Robot Vacuum Cleaner 2](https://xiaomi-mi.com/appliances/xiaomi-mijia-roborock-robot-vacuum-cleaner-2-white) - Robot Vacuum Cleaner
* [Fibaro Multisensor](https://www.fibaro.com/en/products/motion-sensor)
* [Fibaro Relay Switch](https://www.fibaro.com/en/products/switches-2) - Light Switch Control
* [Xiaomi Multifunctional Gateway](https://www.gearbest.com/living-appliances/pp_344667.html) - Gateway was being used for Xiaomi home automation devices. - Now [Zigbee2MQTT](https://github.com/Koenkk/zigbee2mqtt).
* [Xiaomi Window Door Sensors](https://www.gearbest.com/smart-light-bulb/pp_257677.html)
* [Xiaomi Motion Sensors](https://www.gearbest.com/smart-light-bulb/pp_257678.html)
* [Xiaomi Wall Plug](https://www.gearbest.com/living-appliances/pp_344666.html)
* [Xiaomi Wireless Buttons](https://www.gearbest.com/smart-light-bulb/pp_257679.html)
* [Xiaomi Wireless Wall Switch](https://www.gearbest.com/alarm-systems/pp_610095.html)
* [Xiaomi Temperature and Humidity Sensor](https://www.gearbest.com/living-appliances/pp_344665.html)
* [Xiaomi Yeelight RGBW E27](https://www.gearbest.com/smart-lighting/pp_361555.html) - Bedside Lamps
* [Xiaomi Mijia Smart LED Desk Lamp](http://www.gearbest.com/table-lamps/pp_363779.html) - Desk Lamp
* BroadLink SP Mini 3 x4 - Power Socket Control
* [BroadLink RM Mini 3](https://www.gearbest.com/living-appliances/pp_357329.html) - Projector Room Control
* [MiLight WiFi Gateway Emulator](https://github.com/sidoh/esp8266_milight_hub) (NodeMCU ESP8266 / NRF24L01+ module) - Allows for controlling an unlimited amount of LimitlessLED Light groups via MQTT Protocol
* [LimitlessLED Full Color and Dual White Downlight](http://www.limitlessled.com/shop/mr16-rgbw-ww-cw-color-and-white-led) - Smart Dimmable Full Color Downlights
* [LimitlessLED Remote Control](http://www.limitlessled.com/shop/remote-control-for-rgb-ww-cw-color-led-lightbulbs) - Smart Light Remote Control [HASS Integrated](https://github.com/sidoh/esp8266_milight_hub/wiki/Using-Milight-Remote-with-HomeAssistant)
* [Google Home](https://store.google.com/product/google_home) - Voice Assistant/Control
* [Google Home Mini](https://store.google.com/product/google_home_mini) - Voice Assistant/Control
* [Google Chromecast 1](https://www.google.com.au/chromecast/tv/chromecast)
* [Google Chromecast 2](https://www.google.com.au/chromecast/tv/chromecast)
* [Google Chromecast Audio](https://www.google.com.au/intl/en_au/chromecast/audio)
* [Harmony Hub](https://www.logitech.com/en-us/product/harmony-hub?crid=60) - TV and AC Control
* [OwnTracks App](http://owntracks.org) - Mobile Device Tracking
* [Plex Media Server](https://plex.tv) - Media Streaming

# Automations
* Voice Notifications on Google Home's via [Google Assistant Webserver](https://community.home-assistant.io/t/community-hass-io-add-on-google-assistant-webserver-broadcast-messages-without-interrupting-music/37274) on Hassio
* Tensorflow - Notification alerts and Video Recording when people are identified on cameras. [surveillance_cameras.yaml](https://github.com/stanvx/Home-Assistant-Configuration/blob/master/packages/surveillance_cameras.yaml)
* Stream radio stations onto Chromecasts and control their volume.
* On motion from [Fibaro Multisensor](https://www.fibaro.com/en/products/motion-sensor) turn on lights.
* Burgular Alarm from Xiaomi Gateway when alarm panel is Armed and triggered.
* Burgular notifications from [Fibaro Multisensor](https://www.fibaro.com/en/products/motion-sensor)
* Temperature notification from [Fibaro Multisensor](https://www.fibaro.com/en/products/motion-sensor) if no one is home and the home temperature is above 23°C at 5PM. - Option to start the Air Conditioner.
* AC Split System control via [Harmony Hub](http://amzn.to/2n0jhG3).
* Ceiling Fan control via [Broadlink RM Pro](https://amzn.to/2uOoBR0).
* Living Room TV Activity control via [Harmony Hub](http://amzn.to/2n0jhG3).
* Daily Automatic Cleaning when nobody is home via [Xiaomi Roborock Robot Vacuum Cleaner 2](https://xiaomi-mi.com/appliances/xiaomi-mijia-roborock-robot-vacuum-cleaner-2-white)
* [Selective room cleaning](https://community.home-assistant.io/t/howto-xiaomi-vacuum-zoned-cleaning) via [Xiaomi Roborock Robot Vacuum Cleaner 2](https://xiaomi-mi.com/appliances/xiaomi-mijia-roborock-robot-vacuum-cleaner-2-white) including Picture Elements Card card to allow me to click / touch a room to begin a cleaning cycle.
* Automatically lock front door after specific time period.
* Automatically turn on Entryway light when front door opens and turn off after time period.
* Automatically turn on Living room light when front door opens and no motion detected inside for 10 minutes.
* Automatically turn off Outdoor heater after specific time period
* Change Home Assistant to a dark theme at sunset and back to the light theme at sunrise.
* Hide Media Players from the Home Assistant Default View when not being used.
* Media Player light control in Living Room, Dim lights when playing and brighten when paused/stopped.
* [LimitlessLED Remote Control](http://www.limitlessled.com/shop/remote-control-for-rgb-ww-cw-color-led-lightbulbs) forwarding to ensure Home Assistant doesn't lose sync whilst using it.
* Turn on Entryway light for 10 minutes once I get home.
* Weather notification at sunrise and sunset.
* Goodnight script / Voice activation which will turn off all devices, lock the front door and advise via a voice notification if and how many windows or doors are open.
* UPS status notification (On Battery / Low Battery / On Line)
* Trash and Recycle Bin night reminders - Thanks [CCOSTAN](https://github.com/CCOSTAN/Home-AssistantConfig)!
* Washing Machine monitoring and reminders - Thanks [philhawthorne](https://philhawthorne.com/making-dumb-dishwashers-and-washing-machines-smart-alerts-when-the-dishes-and-clothes-are-cleaned/)!
* TV Media Player Control with Picture Elements Card - Thanks [mattclair](https://github.com/mattclair/Home-AssistantConfig)
* NZBGet Downloads Pause when opening streaming apps (Netflix, Youtube, Amazon Prime Video etc.)

# Screenshots
#### Day Theme
![Default](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HA1.PNG)
![Home](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HA2.PNG)
![Security](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HA3.PNG)
![Lights](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HA4.PNG)
![Other](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HA5.PNG)
#### Night Theme
![Night](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HANIGHT.PNG)
#### HA Floorplan
![HA Floorplan](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HAFLOORPLAN.PNG)
#### HA Dashboard
![Home](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HADashboardHome.png)
![Security](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HADashboardSecurity.png)
![Weather](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HADashboardWeather.png)
![Floorplan](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/HADashboardFloorplan.png)

# Photos
![LENOVOTAB4](https://raw.githubusercontent.com/stanvx/Home-Assistant-Configuration/master/screenshots/LENOVOTAB4.png)

Configuration files are being edited with VSCode IDE [Hass.io Add-on](https://github.com/hassio-addons/addon-vscode).

Configuration files are tested against the most stable version of home-assistant using [Travis](https://travis-ci.org/stanvx/Home-Assistant-Configuration).

Message me via the HomeAssistant forums if you have any questions or recommendations in regards to my repository! https://community.home-assistant.io/u/stanvx
