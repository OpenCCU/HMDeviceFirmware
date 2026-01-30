## [HmIP-BBL_update_V1_8_20_201105.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-BBL_update_V1_8_20_201105.tgz)
Required CCU firmware version: &#8805; 3.49.1 / 2.49.1<br/>
<sub>sha256: f0b8bec9b1b97d1d073a48ccdb2894cffbe359a1741d7b69d1949c1a68e47ecf</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:		HmIP-BBL - Homematic IP Blind Actuator for brand switches

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1.8.20 - 2020-11-05
--------------------------------------------------------------

** Bugfix
   * Fix error within production relevant functionality


Version 1.8.16 - 2020-02-06
--------------------------------------------------------------

** Bugfix
   * Fix error within production relevant functionality
   

Version 1.8.10 - 2019-08-15
--------------------------------------------------------------

** Bugfix
   * Motors start briefly even if the profile parameter MAX_TIME_FIRST_DIR is set to 0.0 s
   * HmIP radio shutter and blind actuators can be made to send DeviceInclusions again by a RetriggerDeviceInclusion Request, although this function was only intended for Wired devices
   * If the switch-on and switch-off times in the Easy Profile are set to "Not active" at the same time, the device hangs up
   * Shutters and blinds with longer driving times do not reach end position by short movements (very small values for MAX_TIME_FIRST_DIR)
   * Device does not send a statusinfo if overtemperature was detected

** Improvement
   * Improve switch command functionality by new implementation of local loopback, adding command cancelation and using node sending functionality
   * Modify event counter check to meet current specification
   * If possible, send multicasts only to PARTNER_ALL_WIRED_DEVICES instead of to PARTNER_ALL_DEVICES

   
Version 1.6.2 - 2018-08-09
--------------------------------------------------------------

** Bugfix
   * negative coordinates are not handled correctly
   * incorrect data type order for error status info message
   * default profile for long keypresses is useless
   * problems with automatic measurement of motor delay time
   * missing rf connection leads to stop of local operation at long key presses
   * bug in the creation of direct execution command for the weekprogram
   * actuators trigger, due to the astro function, one hour delayed or prematurely on the day of the time changeover
   
** Improvement
   * new parameter to disable messages to the AC
   * new operation mode for wired devices
   * event counter validation expanded to range
   * slats position now is dominant over the height position if the combination of both is not reachable (near the end positions)
   * all powerup parameters are supported now
   

Version 1.4.10 - 2017-11-30
--------------------------------------------------------------
 
** Bugfix
   * device doesn't send switching commands anymore if a link partner wasn't reachable before.
 
** Improvement
   * added parameter ENDPOSITION_AUTO_DETECT to give the user the opportunity 
     to disable the automatic end position detection if an isolating relay is used.
   * added parameter DELAY_COMPENSATION to give the user the opportunity to use motors 
     with greater delay time between switching the relay and start of motor movement.


Version 1.0.10 - 2017-05-11
--------------------------------------------------------------

** First release


--- END OF FILE ---
