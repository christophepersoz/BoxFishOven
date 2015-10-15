The BoxFishOven controller supports multiple reflow and annealing profiles selectable from the LCD display and a design that makes it easy to add new profiles.

The target oven has two SSRs controlling the top and bottom elements (although we only turn them on/off together), a relay to control the oven's convection fan, and a PWM controlled blower that forces room air into the oven to cool it down rapidly.

Built to run on an Arduino Uno or similar with the Adafruit LCD shield and a MAX31855 thermocouple board, plus transistor/mosfet drivers for all the relays.

**Required Libraries:**
* Arduino PID Library ( https://github.com/br3ttb/Arduino-PID-Library )
* MAX31855 Library for reading the thermocouple temperature ( https://github.com/rocketscream/MAX31855 )

**Included libraries:**
* MenuBackend 1.5 (a modified version of the original MenuBackend 1.4: http://forum.arduino.cc/index.php?topic=38053.45 )
* BoxFishUI (a simple menu driven interface to a 2 line LCD display that uses MenuBackend)
* PIDSeq (a simple PID operations sequencer that uses the Arduino PID Library)

**PID Tuning:**
* http://www.cds.caltech.edu/~murray/books/AM08/pdf/am06-pid_16Sep06.pdf
* http://www.ind-pro-opt.com/Presentations/Practical_Guidelines_for_Identifying_%26_Tuning_PID_Ctl_Loops.pdf

**License:**
* This firmware is released under the Creative Commons Attribution-ShareAlike 4.0
* International license.
* *  http://creativecommons.org/licenses/by-sa/4.0/