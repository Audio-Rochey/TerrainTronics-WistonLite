# WistonLite
A micro version of the Wiston Castle board that uses and external power source.
These come in sets of 10 in a strip that can be separated by hand.

This is heavily based on the Wiston castle board at: https://github.com/Audio-Rochey/TerrainTronics-Wiston-Castle

Changes include:
Battery was removed and solder pads for power up to 5Volts have been added
An additional transistor was added to invert the output, so that the SIG output is GND when there is no magnet present.

Usage notes.
The onboard SL12603 can only drive a small led with up to 10mA or so. Enough for a simple candle, but not enough for more.
Connecting wires to the board is quite simple. There are three solder pads and two holes for an onchip LED.
Add some solder to each of the pads, then when ready, heat up the solder, slide some thing guage wire (wire wrap wire for example), slide the wire into the solder and remove the soldering iron to let the solder cool and harder, holding the LED on!

There are three solder pads on the board, flipping the board over shows which ones are which. 
SIG = Normalized logic out (no magnet = 0V, magnet = vdd)
VDD = Power supply. Anythhing from about 3V up to 5V
GND. 

If you just want a simple LED output, then solder your LED to the two holes on the board. The hole nearest the solder pads is the negative (short wire of the led) and the one furthest from the solder pads is the positive.



