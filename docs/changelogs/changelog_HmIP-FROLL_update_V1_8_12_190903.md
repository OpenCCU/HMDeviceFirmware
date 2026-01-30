## [HmIP-FROLL_update_V1_8_12_190903.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-FROLL_update_V1_8_12_190903.tgz)
<sub>sha256: 0bdbd01f5e09745aa4f04d9baec983879db91171cfc27dbcc2cb144d3ae71052</sub>
Required CCU firmware version: &#8805; 3.49.1 / 2.49.1

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:		HmIP-FROLL - Homematic IP Shutter Actuator for flush mount

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 1.8.12 - 2019-09-03
--------------------------------------------------------------

** Bugfix
   * negative coordinates are not handled correctly
   * incorrect data type order for error status info message
   * default profile for long keypresses is useless
   * missing rf connection leads to stop of local operation at long key presses
   * bug in the creation of direct execution command for the weekprogram
   * actuators trigger, due to the astro function, one hour delayed or prematurely on the day of the time changeover
   * HmIP radio shutter and blind actuators can be made to send DeviceInclusions again by a RetriggerDeviceInclusion Request, although this function was only intended for Wired devices
   * If the switch-on and switch-off times in the Easy Profile are set to "Not active" at the same time, the device hangs up
   * Shutters and blinds with longer driving times do not reach end position by short movements (very small values for MAX_TIME_FIRST_DIR)
   * Device does not work correctly after overtemperature was detected

** Improvement
   * added parameter DELAY_COMPENSATION to give the user the opportunity to use motors 
     with greater delay time between switching the relay and start of motor movement.
   * new parameter to disable messages to the AC
   * new operation mode for wired devices
   * event counter validation expanded to range
   * all powerup parameters are supported now
   * Improve switch command functionality by new implementation of local loopback, adding command cancelation and using node sending functionality
   * Modify event counter check to meet current specification
   * If possible, send multicasts only to PARTNER_ALL_WIRED_DEVICES instead of to PARTNER_ALL_DEVICES
   

Version 1.2.0 - 2017-05-18
--------------------------------------------------------------

** First release


--- END OF FILE ---
