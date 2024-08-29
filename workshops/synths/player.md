# Assembling a Audio Player

### Materials
- DFR0768 Player Pro media player (pre-soldered)
- USB-C cable
- Mini breadboard
- [Amplifier module](amp.md)

## Assembling the module

Plug your DFPlayer into the breadboard. That's it!

[]

## Loading audio

NOTE: **DO NOT CONNECT USB AND A BATTERY AT THE SAME TIME** It will damage your computer.

To load audio onto the DFPlayer, plug in a USB-C cable and connect it to your computer. It should show up as a storage device. Copy an mp3 file into the folder. If you're going to use more than one file, start them with numbers (`1XXXmp3, 2XXX.mp3, etc`).

The player will run through all the files in the folder and then repeat them.


##

Once powered, the DFPlayer needs a "push" to begin playing, and it will pause if it receives another push. You can do this manually using 




## More information

https://wiki.dfrobot.com/DFPlayer_PRO_SKU_DFR0768

<!--
Disabling the prompt and changing default volume:

- Wire VIN (red), GND (black), RX (to TX orange), and TX (to RX yellow) to FTDI cable
- Use the Arduino IDE
- Select "Arduino Pro or Pro Mini" for the board
- Choose the port
- Open Serial Monitor
- Select "Both NL & CR" and 115200 baud
- type `AT` should response `OK`    
- then `AT+PROMPT=OFF`
- then `AT+VOL=7` (0-10 or ?)
- then `AT+PLAYMODE=1` -- repeat all in folder
-->

