AWind library
-------------
Introduction
------------
AWind (arduino window) is Arduino-library that is intended to simplify the use of touch TFT displays for visualization of sensors data in text or chart form. It is also possible to interact with GUI by the use of display touch feature. 
The library is implemented as general window framework that allows creation of simple GUIs. The GUI is consist of text fields, buttons, chart window and etc. 
Special keyboard window is implemented to provide runtime possibility of changing text fields.
At this moment only TFT with 320x240 resolution on Arduiono Mega is tested, but the library can be adjusted to other display dimensions without big efforts.

Installation
------------
TFT
------------
AWind library for TFT displays is build on top of Henning Karlsen libraries: 
* [UTFT](http://www.rinkydinkelectronics.com/library.php?id=51)
* [UTouch](http://www.rinkydinkelectronics.com/library.php?id=55)

OLED
------------
AWind library for OLED displays is build on top of Adafruit_SSD1306 library
* [Adafruit_SSD1306](https://github.com/adafruit/Adafruit_SSD1306)
* [Adafruit-GFX-Library ](https://github.com/adafruit/Adafruit-GFX-Library)

Uncompress those libraries into  arduinosketchfolder/libraries/ folder

To connect display see descriptions for corresponding hardware and libraries .

The content of awind_full.zip from https://github.com/AndreiDegtiarev/AWind/releases uncompress into arduinosketchfolder/libraries/ folder.

Restart the IDE

Documentation
------------
API documentation: http://andreidegtiarev.github.io/AWind/

Examples
--------
TFT
--------
In the each example folder there is a screen-shots to demonstrate how results should looks like
* [Text](https://github.com/AndreiDegtiarev/AWind/examples/Text): Simple example that demonstrate the basic use of text window + touch interaction
* [Charts](https://github.com/AndreiDegtiarev/AWind/examples/Charts): Simple example that demonstrate the basic use of chart window 
![](examples/Charts/Example.JPG)
* [Oscilloscope](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscope): Simple Oscilloscope with possibility to adjust (in runtime) sample ratio, voltage level and signal length
![](examples/Oscilloscope/Example.JPG)
![](examples/Oscilloscope/Example1.JPG)
* [SensorsMonitor](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/SensorsMonitor): This example is based on my personal application - monitor temperature in my camper (outside, inside, fridge: beer has to be cold :-) and etc.). The sensors in this example work in DEMO-mode and real sensors connections is not needed
![](examples/SensorsMonitor/Example.JPG)
* [Gauges](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/Gauges): This example demonstrates how to use gauge and button controls
![](examples/Gauges/Example.JPG)
* [Dialogs](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/Dialogs): This example demonstrates how handle nested dialogs

![](examples/Dialogs/Example.JPG)
* [Tab control](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/TabControl): This example demonstrates how to work with tab controls

![](examples/TabControl/Example.JPG)
* [Vacuum Pump](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/VacuumPump): This advance example demonstrates how to work with tab controls, timer, how interact with stepper motor, relay and etc.

![](examples/VacuumPump/VacuumPump.JPG)

* [Window selector](https://github.com/AndreiDegtiarev/AWind/examples/Oscilloscopeexamples/WindowSelector): This example demonstrates how to control child window visibility

![](examples/WindowSelector/Example.JPG)
OLED
--------
* [GfxOLED_DHT](https://github.com/AndreiDegtiarev/AWind/tree/master/examples/GfxOLED_DHT): interaction with DHT sensor
* [GfxOLED_Oscilloscope](https://github.com/AndreiDegtiarev/AWind/tree/master/examples/GfxOLED_Oscilloscope): simple oscilloscope
* [GfxOLED_SmartCharger](https://github.com/AndreiDegtiarev/AWind/tree/master/examples/GfxOLED_Oscilloscope): smart NiMH battery charger
