RFID Library
============

125Khz RFID library for Arduino. 

This library only support TTL RS232 serial port.

![125Khz RFID Reader][RFID Image]

When read the data from some RFID card, you will get data like `00 91 6f 0b f5`.

Example:
```
your card number: 0009531147
that your data  : 00 91 6f 0b f5
```
**Notice, f5 is the check bit**

`f5 = 00^91^6f^0b`


#### Pins 

1. VCC support 3.3 ~ 5V
2. TX, RX connect to Arduino or Seeeduino
3. T1, T2 is the Signal port for RFID antenna
4. W0, W1 is for wiegand protocol, but this library not support yet.

```
		+-----------+
	----|VCC	  T1|----
	----|GND	  T2|----
	----|TX		 SER|----
	----|RX		 LED|----	
	----|W0		BEEP|----
	----|W1		 GND|----
		+-----------+

```

### Usage
```

```


----

This library is written by [Ye Xiaobo][Github Homepage] for seeed studio<br>
and is licensed under [The MIT License](https://github.com/yexiaobo-seeedstudio/RFID_Library/blob/master/LICENSE). <br>

Contributing to this software is warmly welcomed. You can do this basically by<br>
[forking](https://help.github.com/articles/fork-a-repo), committing modifications and then [pulling requests](https://help.github.com/articles/using-pull-requests) (follow the links above<br>
for operating guide). Adding change log and your contact into file header is encouraged.<br>
Thanks for your contribution.

Seeed Studio is an open hardware facilitation company based in Shenzhen, China. <br>
Benefiting from local manufacture power and convenient global logistic system, <br>
we integrate resources to serve new era of innovation. Seeed also works with <br>
global distributors and partners to push open hardware movement.<br>


[RFID Image]: http://www.seeedstudio.com/wiki/images/6/6a/RFID.jpg
[Github Homepage]: https://github.com/yexiaobo-seeedstudio
