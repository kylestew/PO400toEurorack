# Pocket Operator 400 to Eurorack Conversion

## WARNING ##

I DO NOT RECOMMEND using this conversion as is with most modular setups. The PO-400 modules appear to be picky about their power supply and don't have the standard filtering and voltage spike protection that a standard Eurorack module contains. A noisy startup might fry one of your modules.

A possible solution to this would be adding a fuse and filter circuit to the bus breakout. I'm open to pull requests if someone would like to design this.

![](placed_modules.jpg)

The PO 400 from [Teenage Engineering](https://teenage.engineering/products/po/modular) is Eurorack compatible! Unfortunately [these](https://teenage.engineering/_img/5c40d68837f9710004314dd3_original.pdf) are all the technical details I can find.

#### Known:

+ PO operates in +12V / -12V Eurorack ranges
+ Modules on the PO 400 fit nicely in Eurorack standard sizes (with added faceplates)

#### Unknown:

+ How picky are the modules about their power requirements?
+ Do the CV ranges play nice with standard Eurorack modules?
+ How compatible are the stereo TRS jacks with most Eurorack modules?

#### Assumptions

I'm assuming 12v / -12v from a standard Eurorack PSU is compatible with the PO modules. Voltage is voltage is voltage (I suppose). Given these run off AAs, I'm assuming the amperage is low (maybe I'll measure them later). I'm also trying not to worry about the stereo to mono situation. I may be ordering a lot of conversion jacks soon.

_Update: PO 400 modules work pretty well with standard modules, though some of the CV ranges lack the full range of
usefulness you might be used to._

## Conversion
Two differences need to be addressed before dropping your PO 400 modules into a standard Eurorack format system.

1. Power headers are not compatible
2. Modules are not mountable (too small, wrong hole spacing)

I've cheated on #1 (as you will see). For #2 I've uploaded my design files for laser cutting. These designs are based on the Teenage Engineering [details](https://teenage.engineering/_img/5c40d68837f9710004314dd3_original.pdf) and a lot of measuring. Initial test work great. I cut 3 mm acrylic and realized my Eurorack skiff machine screws are too short to bolt the modules down. Keep this in mind if you're not doing thin wood or metal faceplates.

#### Power Conversion

I hardwired a section of the PO 400 bus to my Eurorack power bus. The PO modules are pretty shallow, there is still room to place them in a Make Noise skiff with the bus added as shown.  

As stated before, a power spike supression circuit should be added here. I've gotten away without it because I have a simple modular setup with few modules likely to dirty up the supply.

I wouldn't recommend cutting the bus as I did or hard wiring it to your Eurorack's bus. We should design a converter modules, pull requests are welcome!

![](bus_mod.jpg)
![](installed_bus.jpg)


_Note to Teenage Engineering, please send a kind note to remove your branding if you feel the need. Big fan of your work, I will do so promptly. Also, thanks for the fun modules!_

