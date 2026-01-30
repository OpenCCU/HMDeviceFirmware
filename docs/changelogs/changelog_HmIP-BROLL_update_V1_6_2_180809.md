## [HmIP-BROLL_update_V1_6_2_180809.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-BROLL_update_V1_6_2_180809.tgz)
<sub>sha256: c3fa44d441f8151f5dc3bbda8c09bd80b094b15adce85cd684494cf7411e4e73</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.31.4

ï»¿Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2/3 ab Version 2/3.31.4
Nach dem erfolgreichen Ãbertragen des Updates ist es erforderlich den HmIP-BROLL einmal von der CCU2 ab- und wieder anzulernen, damit alle neuen Funktionen in der CCU2 korrekt angezeigt werden.

Please note: Only use the firmware file in connection with the CCU2 from version 2/3.31.4
After the update has been successfully transferred, it is necessary to disconnect the HmIP-BROLL from the CCU2/3 and teach-in the device again. So that all new functions are displayed in the CCU2.

Changelog: HmIP-BROLL

Version 1.6.2 - 20180809
--------------------------------------------------------------
Version:
  Application:  1.6.002
  Bootloader:   1.14.000
  Library:      1.32.000
  
** Related Hardware
   * 1714473 + 1714481
   
** Improvement
   * new parameter to disable messages to the AC
   * new operation mode for wired devices
   * event counter validation expanded to range
   * all powerup parameters are supported now
   
** Bugfix
   * negative coordinates are not handled correctly
   * incorrect data type order for error status info message
   * default profile for long keypresses is useless
   * problems with automatic measurement of motor delay time
   * missing rf connection leads to stop of local operation at long key presses
   * bug in the creation of direct execution command for the weekprogram
   * actuators trigger, due to the astro function, one hour delayed or prematurely on the day of the time changeover


Version 1.4.10 - 20171130
--------------------------------------------------------------
Version:
  Application:  1.4.010
  Bootloader:   1.10.000
  Library:      1.20.000

** Related Hardware
   * 1714473 + 1714481
 
** Improvement
   * added parameter ENDPOSITION_AUTO_DETECT to give the user the opportunity 
     to disable the automatic end position detection if an isolating relay is used.
   * added parameter DELAY_COMPENSATION to give the user the opportunity to use motors 
     with greater delay time between switching the relay and start of motor movement.

** Bugfix
   * device doesn't send switching commands anymore if a link partner wasn't reachable before.


Version 1.0.10 - 20170511
--------------------------------------------------------------
Version:
  Application:  1.0.010
  Bootloader:   1.10.000
  Library:      1.20.000

** Related Hardware
   * 1714473 + 1714481
