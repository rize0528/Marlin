# D-Force mini basic metrics

| ID | Variables          | Values       |
|:---|:-------------------|:-------------|
| 1  | DELTA_HEIGHT       | 235.29(+0.5) |
| 2  | DELTA_DIAGONAL_ROD | 262.600      |
| 3  | DELTA_RADIUS       | 110          |
| 4   | <Horizontal radius>                   | 127.950             |

* For DELTA_DIAGONAL_ROD check
https://chenfuguo.gitbooks.io/3d-printing/content/3D_printers/Delta_printer_Calibrating.html

* For Z-Probing (BLTouch) check https://www.antclabs.com/bltouch

D-Force mini stock firmware version is

`READ: FIRMWARE_NAME:Repetier_0.91
FIRMWARE_URL:https://github.com/repetier/Repetier-Firmware/
PROTOCOL_VERSION:1.0 MACHINE_TYPE:Delta EXTRUDER_COUNT:1
REPETIER_PROTOCOL:2`

Use `M115` to acquire above firmware information.

## Tuning

### Gcodes
* M119
  * To test the endstops works or not.

## Tutorials

* [Wiring 3D Printer RAMPS 1.4](https://www.instructables.com/Wiring-3D-Printer-RAMPS-14/)


## Value dumped from stock firmware `M503`
<pre>
READ: EPR:2 75 115200 Baudrate
READ: EPR:3 129 2059.975 Filament printed [m]
READ: EPR:2 125 2050290 Printer active [s]
READ: EPR:2 79 0 Max. inactive time [ms,0=off]
READ: EPR:2 83 120000 Stop stepper after inactivity [ms,0=off]
READ: EPR:3 11 80.0000 Steps per mm
READ: EPR:3 23 300.000 Max. feedrate [mm/s]
READ: EPR:3 35 80.000 Homing feedrate [mm/s]
READ: EPR:3 39 20.000 Max. jerk [mm/s]
READ: EPR:3 133 -105.000 X home pos [mm]
READ: EPR:3 137 -105.000 Y home pos [mm]
READ: EPR:3 141 0.000 Z home pos [mm]
READ: EPR:3 145 105.000 X max length [mm]
READ: EPR:3 149 105.000 Y max length [mm]
READ: EPR:3 153 235.287 Z max length [mm]
READ: EPR:3 59 2500.000 Acceleration [mm/s^2]
READ: EPR:3 71 3000.000 Travel acceleration [mm/s^2]
READ: EPR:3 881 262.600 Diagonal rod length [mm]
READ: EPR:3 885 127.950 Horizontal radius [mm]
READ: EPR:3 925 110.000 Max. radius [mm]
READ: EPR:1 891 70 Segments/s for travel
READ: EPR:1 889 200 Segments/s for printing
READ: EPR:1 893 0 Tower X endstop offset [steps]
READ: EPR:1 895 0 Tower Y endstop offset [steps]
READ: EPR:1 897 0 Tower Z endstop offset [steps]
READ: EPR:3 901 210.000 Alpha A(210):
READ: EPR:3 905 330.000 Alpha B(330):
READ: EPR:3 909 90.000 Alpha C(90):
READ: EPR:3 913 0.000 Delta Radius A(0):
READ: EPR:3 917 0.000 Delta Radius B(0):
READ: EPR:3 921 0.000 Delta Radius C(0):
READ: EPR:3 933 0.000 Corr. diagonal A [mm]
READ: EPR:3 937 0.000 Corr. diagonal B [mm]
READ: EPR:3 941 0.000 Corr. diagonal C [mm]
READ: EPR:0 880 0 Autolevel active (1/0)
READ: EPR:0 106 1 Bed Heat Manager [0-3]
READ: EPR:0 107 130 Bed PID drive max
READ: EPR:0 124 80 Bed PID drive min
READ: EPR:3 108 196.000 Bed PID P-gain
READ: EPR:3 112 33.000 Bed PID I-gain
READ: EPR:3 116 290.000 Bed PID D-gain
READ: EPR:0 120 255 Bed PID max value [0-255]
READ: EPR:3 200 139.000 Extr.1 steps per mm
READ: EPR:3 204 200.000 Extr.1 max. feedrate [mm/s]
READ: EPR:3 208 20.000 Extr.1 start feedrate [mm/s]
READ: EPR:3 212 5000.000 Extr.1 acceleration [mm/s^2]
READ: EPR:0 216 3 Extr.1 heat manager [0-3]
READ: EPR:0 217 255 Extr.1 PID drive max
READ: EPR:0 245 60 Extr.1 PID drive min
READ: EPR:3 218 7.0000 Extr.1 PID P-gain/dead-time
READ: EPR:3 222 2.0000 Extr.1 PID I-gain
READ: EPR:3 226 40.0000 Extr.1 PID D-gain
READ: EPR:0 230 255 Extr.1 PID max value [0-255]
READ: EPR:2 231 0 Extr.1 X-offset [steps]
READ: EPR:2 235 0 Extr.1 Y-offset [steps]
READ: EPR:1 239 1 Extr.1 temp. stabilize time [s]
READ: EPR:1 250 195 Extr.1 temp. for retraction when heating [C]
READ: EPR:1 252 5 Extr.1 distance to retract when heating [mm]
READ: EPR:0 254 255 Extr.1 extruder cooler speed [0-255]
</pre>