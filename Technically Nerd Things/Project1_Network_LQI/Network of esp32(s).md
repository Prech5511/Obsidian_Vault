This network using the same code in example>>ESP_NOW>>ESP_NOW_network
the first module is
esp32 with CH9102x chip 

the second module is
esp32 with CP2102 chip

and the third module is 
Node32s


there are examples code in Arduino IDE. 
![[Pasted image 20240630185659.png]]


Turned out that the first one is the master, according to its highest priority number:

![[Pasted image 20240702182942.png]]

the second module's view:

![[Pasted image 20240702183037.png]]

the third module's view:

![[Pasted image 20240702183127.png]]

In master's view: if nothing goes wrong, master will receive 5 messages for each slave 
then summarize every values (totally 10 numbers from 2 slave module) and send it back to every slave:

![[Pasted image 20240702183454.png]]

In slave's view they will greet to each others for every 5 send messages:

![[Pasted image 20240702183803.png]]

So, I do my experiment by unplugging one of the slaves. To see how master responses
what was happened is the network keep running without the unplugged slave.
average number was come from only the presented slave. but in the end, master still send response message to every slave anyway:

![[Pasted image 20240702184043.png]]

When I reconnect the unplugged slave: 
It waited forever to re-join the network,
I need to reset them all to get the lost slave back into the network and start things over again:

![[Pasted image 20240702184204.png]]

In the other slave view while the unplugged slave is absent, it had been sent "Hello!" messages but had no response at all:
![[Pasted image 20240702184614.png]]


Thing is when I unplugged the master device. The slaves are both waited forever
 Any of them would not take in charge and became a new master.  because the code has already defined number of peer devices.
 

![[Pasted image 20240712125910.png]]

Priority comes from mac address
![[Pasted image 20240712125742.png]]