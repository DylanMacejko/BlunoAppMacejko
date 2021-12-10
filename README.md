# BlunoAppMacejko
Fall 2021 Senior Design Project, Team #7 Bladder Sensor

freq_sweep calculates the gain factors based on the input resistor each time it runs. It's the code the team used to test resistors.

calibrate_gain calculates the gain ONCE and simply outputs the line of code that should be used in after_calibration

after_calibration assumes you know what the gain factors are. This is so the user can prepare for having a single set of gain factors for testing

After running calibrate_gain, use the output and paste it into line 13 of after_calibration ( double gain[NUM_INCR+1]={ ... ) If you change any of the input conditions (input resistor, number of points in the sweep, sweep start) the gain factors will no longer be accurate and you should recalculate using calibrate_gain

test23rd is analogous to freq_sweep and test23rdCalibrate is analogous to after_calibration. It removes all output except for outputting the impedance during the sweep. (which it does on 115200 baud)

The Android Studio code is currently in the process of being updated. Since the previous team's work was completed, libraries were updated which changed some of the functionality of the bluetooth connection.
With that being said, we are carefully analyzing the code from the previous repository and changing it to account for the new versions of the libraries provided.
Once changed, the bluetooth functionality should resume and calibration/in-vitro testing will move forwards.
