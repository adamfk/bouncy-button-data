# FAQ
## Do I need to solder wires to my switch?
Alligator clips are fine if you are doing regular testing and your switch is bouncing less than 20ms.

Why the limit of 20ms? If alligator clips are involved and there is significant bounce in the switch, people may attribute the long bounce data to alligator clip movement (which could definitely be the cause).
You can get around this by securing the switch in place so that the alligator clips aren't moving.

If you want to do advanced testing like fast activations or smack tests though, you really do need a very solid connection (soldered, screw, or secure crimp).

## How do I create the summary image?
See https://github.com/adamfk/bouncy-button/tree/main/bbb-browser#tight-export-mode

The important parts are:
1. enable `Tight Export`
2. sort by duration if you think it is helpful
3. capture your screen using whatever method you like
   - on Windows, you can press `ALT+<print_screen>` to capture just your active window (not all monitors)
4. paste the image into the GitHub issue where you want it.

## How do I measure my Arduino's internall pull up resistor?
1. make sure your Arduino is running the bouncy-button-benchmark softare
2. connect a multimeter (DMM) across pin 4 and ground
3. use your DMM to the measure the voltage (it should be around 4.99 volts)
4. use your DMM to measure the current.
5. use ohms law to calculate resistance. R = volts/current.

More details here: https://hackingmajenkoblog.wordpress.com/2016/08/12/measuring-arduino-internal-pull-up-resistors/

