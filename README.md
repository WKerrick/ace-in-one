# The Ace-in-One
The purpose of this project is to make an alternative to acquiring the 2 multitaps and additional controllers needed for ACE speedruns like 0 Exit in Super Mario World. This device mimics having multitaps plugged into both port 1 and 2, with a controller in the first two ports of each multitap. Instead of using clamps and other items to hold down buttons on the additonal controllers, DIP switches are used instead.


## Production
You can use the Gerber, BOM, and Pick-n-Place files to have a PCB manufacturer build the board for you. I personally use JLCPCB, but there are many boardhouses out there for you to choose from.


## Addtional Items
* 1 SNES Controller Connector (female)
* 3 DIP Switches (12P)
* 2 Output Connectors (options described below)
* Output Cables (24awg6c or 26awg7c)
* 2 SNES Controller Connectors (male)
* 1 Arduino Nano (optional)


## Output Connectors
The Ace-in-One can 3 different styles of connector you can use for output. Make sure you have the required hardware for your output of choice, including any crimpers that are needed.

1. 0.1" 6P (for headers or standard auto connectors)
2. 2mm 6P (for JST_PH connectors)
3. 2mm 7P (in case you're like me and have 7P cables pre-made for other devices)


## Pinouts
### Arduino Nano
 Pin | Name
---- | ----
6 | Clock
3 | Latch
4 | Data1

### Output Port 1
 Pin | Name
---- | ----
1 | 5v
2 | Clock
3 | Latch
4 | Data1
5 | Data2
6 | [UNUSED]
7 | Ground

### Output Port 2
 Pin | Name
---- | ----
1 | 5v
2 | Clock
3 | Latch
4 | Data3
5 | Data4
6 | [UNUSED]
7 | Ground


## Notes
If adding Arduino, make sure to solder the middle DIP first, followed by the arduino, and then the other 2 DIP switches— otherwise it'll be a tight squeeze.

Any questions or comments can be sent to discord (WKerrick#0258) or twitter (w_kerrick)