sony_slink
==========

This Arduino sketch is entirely based on the great work from 
These are Arduino sketches to interface with Sony equipment using the
S-Link/Control A1 protocols. There are two sketches here:
* Target Arduino, USB serial communication
* Target ESP8266, wifi + websocket communication

I'm using this to control and read information from a Sony CDP-CX225 CD Player.

To physically connect an Arduino device to the S-Link bus you need
some additional components. Here's a schematic for the Arduino (ESP8266 is similar, but uses different pins):

![circuit](circuit.png)

Use a 3.5 mm mono plug to connect the Arduino/ESP8266 to the S-Link/Control A1 port of the Sony equipment and connect the Arduino to a USB port in your computer for power and serial communication.

The S-Link_CDP-CX225.ods file lists the commands I have found work with the CDP-CX225.

----

Reference documents:
* http://web.archive.org/web/20070720171202/http://www.reza.net/slink/text.txt
* http://web.archive.org/web/20070705130320/http://www.undeadscientist.com/slink/
* http://web.archive.org/web/20180831072659/http://boehmel.de/slink.htm
