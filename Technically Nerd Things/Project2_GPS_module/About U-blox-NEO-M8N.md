First things: I recommend you to install support-software called "u-center" from their website
[u-center | u-blox](https://www.u-blox.com/en/product/u-center)
In my case, my device is version 8 (knowing from its name M8N), then I chose this version.
https://content.u-blox.com/sites/default/files/2024-06/u-centersetup_v24.05.zip
if you have 10 or higher version, you must install this one instead.
https://u-center2-updates.u-blox.com/u-center2-installer.exe

You can use their software to configure many things here. There a lot of information getting from this module and they are virtualized to understand easily.

You also need an "TTL connector" to connect between your u-blox module and your pc
using "USB MINI B" to "USE TYPE A" cable 
![[Pasted image 20240630180514.png]]

or you just need other type of TLL connector like I did, in My experiment/Test NEO-M8N
![[Pasted image 20240630180703.png]]


![[Pasted image 20240630164341.png]]

this video guide me how to connect wires. 
[Configure GPS Modules With Ucenter (youtube.com)](https://www.youtube.com/watch?v=eRxLyReDY5A)

or follow this picture
![[Pasted image 20240630180745.png]]

Interesting project with esp32
Using esp32 and u-blox module to receive GPS signal and send it to your android phone via Bluetooth connection. Unfortunately, There is no code file given.
https://youtu.be/Y02c3gsoqLU?si=PgEH4XDj1rv92lNm

#### *But there are suspects that some of U-blox module buying from online-sources are fake modules! There are many forums telling you if your module is likely to be a fake one or not.


https://portal.u-blox.com/s/question/0D52p00008HKCf6CAH/not-a-real-m8n-i-think
https://rtklibexplorer.wordpress.com/2016/12/06/counterfeit-m8n-modules/
https://portal.u-blox.com/s/question/0D52p00008HKEEECA5/psa-fake-ublox-modules-and-potential-ways-to-identify-them
https://youtu.be/2qPivbIXfQE?si=_CqNeyMnv1cEUZNk
https://youtu.be/buyFIcgee5w?si=XZnfwZaRGnzJY75D

For sum, Fake modules can't update their firm ware because there is no physical flash memory under their cover. It's true that I can't configure any thing into my flash memory inside my module using u-center software. They always notify me with error message. I won't dare to open its cover  myself to confirm the fact. Sorry, I suppose that my module is fake after all. 
Still, It works.

#### An interesting Topic to discuss 
https://youtu.be/FmdG66kTfsI?si=tzGdnp8XLsl3brOa
He do an experiment to compare between version6 and version8 which is different in number of satellite system that capable of receiving signal from them.
for summary, there not much difference from each others. they are depend on your luck to do your observation on the right time and hope that there are many satellites on above your head to get more accurate and stable positioning measurement from your module. He adds that measuring height from both module are bad compare to height measured from pressure sensor.