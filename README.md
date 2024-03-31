# WistonLite
A micro version of the Wiston Castle board that uses and external power source.
These come in sets of 10 in a strip that can be separated by hand.

This is heavily based on the Wiston castle board at: https://github.com/Audio-Rochey/TerrainTronics-Wiston-Castle
![IMG_2846](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/66a2c220-09e9-4553-8dd4-beda2eb795a1)

Changes include:
Battery was removed and solder pads for power up to 5Volts have been added
An additional transistor was added to invert the output, so that the SIG output is GND when there is no magnet present.

# Maximum Voltages etc
- Maximum Input Power Voltage is 5V.
- Minimum Input Power Range is 2V. (So, using a coin CR2032 battery should be fine)
- Maximum output Current is about 5mA. (enough for 1 LED). If more power is needed, a Carew Castle LED Cloner can be used to drive up to 2Amps of current!

## Usage notes.
The onboard SL12603 can only drive a small led with up to 5mA or so. Enough for a simple candle, but not enough for more.
Connecting wires to the board is quite simple. There are three solder pads and two holes for an onchip LED.
Add some solder to each of the pads, then when ready, heat up the solder, slide some thing guage wire (wire wrap wire for example), slide the wire into the solder and remove the soldering iron to let the solder cool and harder, holding the LED on!

There are three solder pads on the board, flipping the board over shows which ones are which. 
![SuperCloseUpWL](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/e1133bd1-ba6f-4ced-bba7-68cb42df593c)

SIG = Normalized logic out (no magnet = 0V, magnet = vdd)
VDD = Power supply. Anythhing from about 3V up to 5V
GND. 

### Simple LED Output

If you just want a simple LED output, then solder your LED to the two holes on the board. 
![LEDPinoutWL](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/1bd0ee30-6e3a-4084-ba4d-0eeffe730e88)

The hole nearest the solder pads is the negative (short wire of the led) and the one furthest from the solder pads is the positive.

### Drici



