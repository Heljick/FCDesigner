# FCDesigner
Patch to use FadeCandy board with TouchDesigner
Tested with vserion 58620 and some olders of TouchDesigner without any issues

Python:
Before all you need to install Python as you may have some issue with the Python library on TouchDesigner. The system has been tested with 3.3 and 3.5.1 but should works with others versions. 
Download Python here:https://www.python.org/downloads/
Install Python in "c:/Python"
In TouchDesigner "Edit->Preferences", select "Add external Python to search path", select "c:/Python/Lib" and click "Apply" at the bottom 

FCServer:
Put all the files in FCServer folder on your desktop and launch "FCServer.bat" to start the server
You need to configure "conf.json" to fit your LED configuration and restart FCServer every time you make any change.
If you don't know how to configure "conf.json", here is an explanation https://learn.adafruit.com/1500-neopixel-led-curtain-with-raspberry-pi-fadecandy/fadecandy-server-setup

OPC:
The "OPC.py" in OPC folder need to be put in "C:\Program Files\Derivative\TouchDesigner088\bin\Lib"

Launch FCDesigner:
When everything is installed, launch "FCServer.bat" to start the server, connect your FadeCandy to your computer and it should appear on FCServer.
Now you can launch "FCDesigner.toe" and start to play with your LEDs and TouchDesigner.

!!! FCserver must be launch before TouchDesigner or you can experiment several performance downgrade, if It's the case, just launch FCServer, no need to restart TouchDesigner. 

Other links: 
TouchDesigner donwload -> https://www.derivative.ca/088/Downloads/
FadeCandy project -> download Touch from: https://www.derivative.ca/088/Downloads/
FadeCandy google forum -> https://groups.google.com/forum/#!forum/fadecandy
FCDesigner forum -> coming soon

My work is based on TouchCandy patch https://github.com/Swaeg/TouchCandy by Marko Vierimaa, PixelMappingGeo.2.toe by Dudley Smith and of curse Micah Scott's work who created the FadeCandy. You can found all the contributors who was working before me on this project here https://groups.google.com/forum/#!topic/fadecandy/5vY-NFpYs6c
