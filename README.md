This project requires:

a way to send your channel stats via mqtt , i used NODERED to extract them and throw them out in mqtt

i used esphome 

1x esp8266 wemos d1 mini lite
4x max7219 7 segment 6 digit display in chain.

wiring.
open readme in code so the formatting isnt poop


on the WMOS D1:
D1                          [ DISPLAY 1 ]        
5v ------------------> VCC                VCC--------- etc    display 2    display 3            display 4
GND------------- ----> GND  [ yt views  ] GND--------- etc    yt subs      twitch followers     twitch subs
D7 ------------------> DIN                DOUT-------- etc
D8 ------------------> CS                 LODA-------- etc
D5 ------------------> CLK                CLK--------- etc


the last display may be dim and may need its its own 5v line
