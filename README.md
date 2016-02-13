# d3vice
Airsoft multi-device distributed system

This is a documentation repository. For the individual parts, see the respective repos:

* [D3vice Gameserver][0]
* [D3vice Raspberry Pi Sensor][1]
* [D3vice WebUI][2]



## Specs

### ESP8266 sensor

#### Bootstrapping

This is for end user configuration. It's a way for the ESP8266 to join a WLAN without having to hard code WIFI auth info

* starts as open wifi AP
* end user connects to wifi AP using their phone
* end user navigates to very simple ESP8266 web ui, enters non-unique D3vice configuration password (prevent casual mischief)
* in web ui, user sets username and password for the WPA2 network D3vice will be running on.
* save
* ESP8266 joins wifi network.
* If unsuccessfull join, reverts back to AP mode and process can repeat


[0]:https://github.com/doomsquadairsoft/d3vice-gameserver
[1]:https://github.com/doomsquadairsoft/d3vice-rpi-sensor
[2]:https://github.com/doomsquadairsoft/d3vice-client
