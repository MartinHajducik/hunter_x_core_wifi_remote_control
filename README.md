# Hunter X-Core irrigation controller - home made wifi remote control

https://www.hunterindustries.com/en-metric/irrigation-product/controllers/x-coretm 

This project is was inspired by Claude Loullingen , you can find more details here http://www.loullingen.lu/projekte/Hunter/index.php?language=EN . 
Only difference is Basic HTTP authentication in case you want secure wifi controller webserver -> expose it to the Internet.

I am using Espressif ESP32 board. You can find cable wiring on picture below.

Only what you have to change in source code are constants : 

ssid - Name of your WiFi network
password - Password to you wifi network
http_username - Username for webserver in order to authenticate against frontend or API 
http_password - Password for webserver in order to authenticate against frontend or API 


How to make it run , step by step: 

1) Download source code


== API ==

It is also possible to control your unit over API

http://<your_ip_address>:<port>/update?zone=<zone_number>&time=<number_from_0_to_240>



