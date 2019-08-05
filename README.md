## Adafruit VCNL4040 Proximity and Lux Sensor PCB

<a href="http://www.adafruit.com/products/4161"><img src="assets/4161.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit VCNL4040 Proximity and Lux Sensor. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4161

### Description

The VCNL4040 is a handy two-in-one sensor, with a proximity sensor that works from 0 to 200mm (about 7.5 inches) and light sensor with range of 0.0125 to 6553 lux.

We've all been there. That thing is _close_ but _how close?_ When you need to measure a small distance with reasonable accuracy, such as the rough height of particularly calm bumble bee, the VCNL4040 Proximity Sensor from Vishay can do that for you. If perchance you also needed to measure the amount of light at the same time, perhaps to let the bee to know if it's time for bed, you're in luck! The VCNL4040 can do that too (bumble bee not included, we tried putting it in the anti-static bag but it started buzzing in a threatening manner)

"OK, _finally_ I can get started on my bee measuring and light sensing project, but _how do I use it_?" you say. To make life easier so you can focus on your important work, we've taken the VCNL4040 and put it onto a breakout PCB along with support circuitry to let you use this little wonder with 3.3V (Feather/Raspberry Pi) or 5V (Arduino/ Metro328) logic levels. Additionally since it speaks I2C you can easily connect it up with two wires (plus power and ground!).  We've even included SparkFun qwiic compatible [STEMMA QT](https://learn.adafruit.com/introducing-adafruit-stemma-qt) connectors for the I2C bus so **you don't even need to solder!** [Just wire up to your favorite micro and you can use our CircuitPython/Python or Arduino drivers to easily interface with the VCNL4040 and make approximate approximations of proximity in no time!](https://learn.adafruit.com/adafruit-vcnl4040-proximity-sensor/)

To give you some ability to tune your measurements for your situation, the VCNL4040 lets you adjust the integration time (how long light is being measured) to set the sensitivity of your measurements depending on the lighting conditions. With an integration time of 80ms, since the sensor is only collecting measurements for a short period of time, each measured bit of light represents a larger amount of light. For this reason the maximum range in lux for the 80ms integration time is 6553.5 lux.

If you use a longer integration time and get the same amount of light measurements "events", you know that there is comparatively less light because we're waiting around longer for light to show up and getting the same number, meaning the rate of light events is lower. For this reason at the maximum integration time of 640ms the VCNL4040 will only measure up to 819.2 lux.

It is also worth keeping in mind that as you increase the integration time you are also increasing the sensitivity and resolution within the measurement range

In addition to adjusting the sensitivity of light measurements, you can change the current and duty cycle of the IR LED that powers the proximity detection to adjust how sensitive proximity measurements are
### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Kattni Rembor for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
