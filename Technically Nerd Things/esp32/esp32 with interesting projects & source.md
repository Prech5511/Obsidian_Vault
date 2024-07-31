I recommend this website which contain many code example for microcontroller projects
"DroneBot Workshop"
[Tutorials & Projects | DroneBot Workshop | Arduino & Raspberry Pi](https://dronebotworkshop.com/)
In this case, let's focus on esp32
[ESP NOW - Peer to Peer ESP32 Communications (dronebotworkshop.com)](https://dronebotworkshop.com/esp-now/)
the owner himself has recorded a video about this project.
https://youtu.be/bEKjCDDUPaU?si=BZZCUp14B8TjmkKH


Another of my recommend source is here.
[Control ESP32 and ESP8266 GPIOs from Anywhere in the World | Random Nerd Tutorials](https://randomnerdtutorials.com/control-esp32-esp8266-gpios-from-anywhere/)

#### Control ESP32 and ESP8266 GPIOs from Anywhere in the World
Using esp32 to control a device remotely . Create connection between database and esp32. Use its API and your WIFI SSID. Then Get UI controlling interface.
https://youtu.be/4moPYxNYjCY?si=uOf_4_cpKew5-zEV


There is esp-now (protocol for communication among esp32s)
[Getting Started with ESP-NOW (ESP32 with Arduino IDE) | Random Nerd Tutorials](https://randomnerdtutorials.com/esp-now-esp32-arduino-ide/)
[ESP-NOW with ESP32: Send Data to Multiple Boards (one-to-many) | Random Nerd Tutorials](https://randomnerdtutorials.com/esp-now-one-to-many-esp32-esp8266/)
someone do a video about this
https://youtu.be/cYqaphpWxwI?si=Mpfv0Qh2s7woOEgT
I have tried it.
from my understanding, They don't use your WIFI as an access point. They use their own protocol. But still use specific MAC address of receiver (assigned esp32). 
![[Pasted image 20240630190636.png]]
The one equipped with extension board is transmitter.
![[Pasted image 20240630190647.png]]

there are other example code in Arduino IDE. These are boardcasting method.
![[Pasted image 20240630185659.png]]



