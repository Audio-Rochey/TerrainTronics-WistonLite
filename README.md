# WistonLite
A micro version of the Wiston Castle board that uses and external power source.
These come in sets of 10 in a strip that can be separated by hand.
<!-- ![WistonLiteStrip](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/ce2840ee-6b05-42fa-af4e-04f0be25f22c) -->

<img src="https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/ce2840ee-6b05-42fa-af4e-04f0be25f22c](https://github-production-user-asset-6210df.s3.amazonaws.com/15720888/318277969-ce2840ee-6b05-42fa-af4e-04f0be25f22c.jpg" width="400" >

This is heavily based on the Wiston castle board at: https://github.com/Audio-Rochey/TerrainTronics-Wiston-Castle


<img src="https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/66a2c220-09e9-4553-8dd4-beda2eb795a1.JPEG" width="400" >
<!-- ![IMG_2846](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/66a2c220-09e9-4553-8dd4-beda2eb795a1) -->

Changes include:
Battery was removed and solder pads for power up to 5Volts have been added
An additional transistor was added to invert the output, so that the SIG output is GND when there is no magnet present.

# Maximum Voltages etc
- Maximum Input Power Voltage is 5V.
- Minimum Input Power Range is 2V. (So, using a coin CR2032 battery should be fine)
- Maximum output Current is about 5mA. (enough for 1 LED). If more power is needed, a Carew Castle LED Cloner can be used to drive up to 2Amps of current!

## Usage notes.
The onboard SL12603 magnetic sensor can only drive a small led with up to 5mA or so. Enough for a simple candle, but not enough for more.
Connecting wires to the board is quite simple. There are three solder pads and two holes for an onchip LED.
Add some solder to each of the pads, then when ready, heat up the solder, slide some thing guage wire (wire wrap wire for example), slide the wire into the solder and remove the soldering iron to let the solder cool and harder, holding the LED on!

There are three solder pads on the board, flipping the board over shows which ones are which. 
<!-- ![SuperCloseUpWL](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/e1133bd1-ba6f-4ced-bba7-68cb42df593c) -->
<img src="https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/e1133bd1-ba6f-4ced-bba7-68cb42df593c.jpg" width="400" >

- SIG = Normalized logic out (no magnet = 0V, magnet = vdd)
- VDD = Power supply. Anything from about 2V up to 5V
- GND = Ground, Lower voltage supply, Common. 

## How to solder these pads.

I use wire wrap wire (That's 30AWG wire), trim about 3mm of plastic off.

![solderpadgif](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/8db2dec7-ce0c-461a-91b3-e9817edf827c)


Then add a blob of solder to the pad (might take a little flux to get it to flow nicely) then:
- heat up the blob of solder
- slide in the end of the wire
- remove heat and allow the wire to cool in the solder.

# Uses and How to connect them up.
For ideas on how to connect this board together and use it in your terrain builds, see below.

## One single, simple LED Output
If you just want a simple LED output, then solder your LED to the two holes on the board. 
![LEDPinoutWL](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/1bd0ee30-6e3a-4084-ba4d-0eeffe730e88)

The hole nearest the solder pads is the negative (short wire of the led) and the one furthest from the solder pads is the positive.

## Connection to a Wemos D1 or Arduino for larger puzzle rooms.
Care should be taken in doing this.
### Wemos D1:
WistonLite should be powered with the same voltage as your Microcontroller/Arduino. For example, the Wemos D1 Mini actually runs from 3.3V, even though it's a USB powered device. Each of it's input and output pins operates from 3.3V. Therefor, your WistonLite should be powered from the 3.3V pin on the Wemos D1.
### Arduino Uno:
![Arduino Hookup Thumbnail](https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/2f6bcb55-c5b5-4207-aca2-be6837f81ccc)

Link to larger size: (https://github.com/Audio-Rochey/TerrainTronics-WistonLite/assets/15720888/2b3d42ee-59e1-4d55-b634-384c4f61a230.jpg)

Arduino UNO's digital input pins handle up to 5V. Therefor, you can power your Wiston Castle from the 5V pin.

# Schematic and High Level "How it works"

## Schematic

## Theory of operation





