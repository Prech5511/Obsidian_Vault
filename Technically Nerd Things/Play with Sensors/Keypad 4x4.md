![[Pasted image 20240711160821.png]]![[Pasted image 20240711160829.png]]![[Pasted image 20240711160857.png]]

due to different pin position of Node32s I need to change pin number in these 2 list(s)
Library named "keypad" are required.

again, the source code is here.
[Using Keypads with Arduino - Build an Electronic Lock (dronebotworkshop.com)](https://dronebotworkshop.com/keypads-arduino/)

![[Pasted image 20240711161219.png]]
face the keypad up, the order of pin you need to configure will be:
1. Row 1
2. Row 2
3. Row 3
4. Row 4
5. Column 1
6. Column 2
7. Column 3
8. Column 4
numbers start from left to right as 1- 8

So, I connected the previous project with my KY-008 laser module. I just disable any line that refer to LCD display which I didn't use. Then define pin 13 to control the laser output instead of relay. Finally, I initialize Serial with 9600 baud to know what I press in serial monitor. When I put a correct password via keypad, laser module will be turned on for 5 seconds.
![[Pasted image 20240711170040.png]]
![[Pasted image 20240711171133.png]]