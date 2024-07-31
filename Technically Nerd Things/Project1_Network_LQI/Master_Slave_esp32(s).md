There is esp-now (protocol for communication among esp32s)
[Getting Started with ESP-NOW (ESP32 with Arduino IDE) | Random Nerd Tutorials](https://randomnerdtutorials.com/esp-now-esp32-arduino-ide/)
for multiple slave: 
[ESP-NOW with ESP32: Send Data to Multiple Boards (one-to-many) | Random Nerd Tutorials](https://randomnerdtutorials.com/esp-now-one-to-many-esp32-esp8266/)

someone do a video about this
https://youtu.be/cYqaphpWxwI?si=Mpfv0Qh2s7woOEgT
I have tried it.
from my understanding, They don't use your WIFI as an access point. They use their own protocol. But still use specific MAC address of receiver (assigned esp32). 
![[Pasted image 20240630190636.png]]
The one equipped with extension board is transmitter.
![[Pasted image 20240630190647.png]]

there are other example code in Arduino IDE. These are boardcastmethod.
![[Pasted image 20240630185659.png]]

