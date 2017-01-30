# *Blue Pill* Extender

There is a cheap, wildly available STTM3232F103C8T6 board out there. Because of it's shape and color it's called *Blue Pill* (BP). More details about this board can be found on [jeelabs](http://jeelabs.org/article/1649a/).

The board fits perfectly fine in a breadboard but it's missing the convenient programming headers for [SER+](http://jeelabs.org/article/1649f/) and some other features (see list below).

Thanks to the fantastic people over at jeelabs.org I was able to create this add-on board for the *Blue Pill* in KiCAD.

## Features

* Programming header for [SER+](http://jeelabs.org/article/1649f/) including automatic reset of the STM32
* Area for mounting an RFM69-CW module
* Reset button
* Optimized for use on a breadboard

## Current State

Revision 1 is a little bit off-center but working perfectly fine.

There are some plans for the next revision of the board (see *Issues*). Some of them will probably become a completely different board as this one is meant to be used on a breadboard.

## Usage
The *Blue Pill Extender* (BPE) is mounted on top of an existing BP (label facing up).

First prepare the BPE by soldering on the small resistors. The reset button is not required but may be helpful. Also add the RF module if you plan to use one. Make sure the RF module is not placed wrongly!

The 90° programming headers should be mounted from below (soldering on top) but they do work both ways.

Now remove the jumpers from the *BOOT?* pins on the BP and push the BPE on there. Make sure the 2x3 header of the *BOOT?* goes through the BPE and there there is still enough room to plug in an USB cable. Solder the 2x3 headers to the BPE. Now use some short wires (or leftover resistor legs) to connect all the outer BPE pins to the corresponding pins on the BP below – **DO NOT solder the antenna to the BP below!**

## References

* [Ser+ Programming Header](http://jeelabs.org/article/1649f/)
* [RFM69 CW Pinout](https://openenergymonitor.org/emon/sites/default/files/RFM69CW-V1.1_Hope_pinouts.jpg)
* [HyTiny Extener Layout](https://github.com/jeelabs/embello/blob/master/explore/1608-forth/tex/tex-v0.pdf)
* [BP Pinout](http://wiki.stm32duino.com/images/a/ae/Bluepillpinout.gif)
