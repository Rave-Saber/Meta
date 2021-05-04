# Rave Saber

Rave Saber is an open source, open hardware lightsaber build. Unlike most
sabers, which focus on mainly on sound playback - we focus heavily on the
visual effects. Rave sabers are meant to be swung around to the beat of some
loud music :)

Rave Saber uses DotStar LEDs driven with an Atmel ATmega168a AVR
microcontroller.


## Releases

The Hardware & Firmware releases are kept in lockstep - v1 of the firmware
should be used with v1 of the hardware.

### v2.0.0

* [Hardware v2.0.0][hw2.0.0]
* [Firmware v2.0.0][fw2.0.0]

This is the first semi-portable design. Instead of a breadboard & bench power
supply, the components are soldered onto a prototyping board & a voltage
regulator has been added for use with 7.4V Li-Ion betteries.  We've also added
an external oscillator circuit that lets us bump the chip speed from 8Mhz to
16Mhz. There is still no recommended blade or hilt design - we zip-tied our
LEDs, board, & battery to a 1x2 piece of wood.

The firmware now supports rendering patterns in addition to solid colors. There
are pre-defined patterns for flashes, ribbons, bands & scrolls in both RGB &
Rainbow color sequences. If you don't like the patterns pre-defined in our
library, you can write your own as well. Some power-saving optimizations have
been made now that we are limited by battery life, for example, we can limit
the current used by the strip so that all 144 LEDs can be lit without exceeding
the 3A supplied by the power circuit.

### v1.0.0

* [Hardware v1.0.0][hw1.0.0]
* [Firmware v1.0.0][fw1.0.0]

This is pretty much the simplest possible design we could make. It's meant for
prototyping & testing - not for use in a hilt. The hardware is assembled using
a breadboard & powered via a bench power supply, and the firmware allows for
switching between various blade colors.


## License

These licenses apply to every [Rave Saber](https://github.com/Rave-Saber/)
repository:

* **Code:** GPL v3.0
* **Hardware:** CERN OHL v1.2
* **Content/Media:** CC BY-NC-SA v4.0

Feel free to contact us for exceptions.


[hw1.0.0]: https://github.com/Rave-Saber/Rave-Saber-Hardware/tree/v1.0.0
[fw1.0.0]: https://github.com/Rave-Saber/Rave-Saber-Firmware/tree/v1.0.0
[hw2.0.0]: https://github.com/Rave-Saber/Rave-Saber-Hardware/tree/v2.0.0
[fw2.0.0]: https://github.com/Rave-Saber/Rave-Saber-Firmware/tree/v2.0.0
