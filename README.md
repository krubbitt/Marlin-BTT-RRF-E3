# Marlin-BTT-RRF-E3
You can find Marlin firmware for Ender 3 V2 on this repo, anything that you need that i can help just contact me and i´ll try my best to help.

## BIG TREE TECH RRF E3 IT´S NOT COMPATIBLE WITH ENDER 3 V2 OUT OF THE BOX

So the board it´s perfectly compatible with Ender 3 and Ender 3 Pro but not with Ender 3 v2 version because of the screen.

    /**
     *        Ender 3 V2 display                         BTT E3 RRF
     *                _____                                     _____
     *            5V | 1 2 | GND                            5V | 1 2 | GND
     *   (BTN_E1) A  | 3 4 | B (BTN_E2)         (BTN_EN1) PE11 | 3 4 | PB1 (BTN_E2)
     *          BEEP | 5 6   ENT (BTN_ENC)       (BEEPER) PE10 | 5 6   PB2 (BTN_ENC) (needs testing, is boot1)
     *      (RX1) TX | 7 8 | RX (TX1)                    RESET | 7 8 | PE7
     *            NC | 9 10| NC                            PE9 | 9 10| PE8 
     *                -----                                     -----
     *                EXP1                                      EXP1
     */
     
So all the configuration files on the pins for the motherboard can be done except for the   *TX* and *RX* ones that will go on the   TFT pin which is next to the probe connector:

(Image Pendig)

So you have to conect those wires to the pins marked as RX1 and TX1 just carefull with the names because 
>__TX1 goes with RX__

>__RX1 goes with TX__.

## BLTOUCH CONFIG
__

I added my probe offset congif, which are for the Hero Me 5 on the ender 3 V2 with a direct drive adapter, change them as you need.


So i'll try to get everything i can test here which the list right now is:

- [ ] E3 V2 DWIN (factory display)
- [ ] E3 V2 DWIN BLTOUCH (factory display)
- [x] E3 V2 BTT TFT35 E3 V3.0
- [x] E3 V2 BTT TFT35 E3 V3.0 BLTOUCH
- [ ] E3  
- [ ] E3 BLTOUCH 
- [ ] E3 TFT35 E3 V3.0
- [ ] E3 TFT35 E3 V3.0 BLTOUCH
- [ ] E3 PRO  
- [ ] E3 PRO BLTOUCH 
- [ ] E3 PRO TFT35 E3 V3.0
- [ ] E3 PRO TFT35 E3 V3.0 BLTOUCH
