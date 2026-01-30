## [HmIP-FROLL_update_V1_2_0_170523.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-FROLL_update_V1_2_0_170523.tgz)
<sub>sha256: 12642fc668d78953aefca827a98d03dd92084e79ba35ecb6f7bc5930ffb15dd7</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.31.23

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device: HmIP-FROLL - Homematic IP Shutter Actuator for flush mount

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1.2.0 - 20170518
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix
   * device doesn't send switching commands anymore if a link partner wasn't reachable before


Version 1.0.8 - 20170505
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix
   * moving to position doesn't work if the parameter DRIVING_MODE is set to an extreme position and the shutter/blind has already this extreme position


Version 1.0.7 - 20170503
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix
   * status info telegrams are partially longer than the maximum allowed length 


Version 1.0.6 - 20170428
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix 
   * temperature isn't sent at boot
   * RSSI is set in status error telegrams although this is no answer
   

Version 1.0.5 - 20170426
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix 
   * when the configuration button is pressed, the device hangs
   

Version 1.0.4 - 20170425
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix 
   * added missing sending of weekprogram status after inclusion
   * status request doesn't work with weekprogram channel


Version 1.0.3 - 20170419
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469
 
** Bugfix 
   * check if switch time is valid on current day was wrong, so switch times are always valid and are done every day.
   * fixed bug on daylight saving time calculation
   * HmIP-Schalt-/Dimm- und Rollladenaktoren senden ab dem ersten Auftreten einer Antwort mit NACK, nur noch Antworten mit NACK 
   * a switching command is now correctly answered with status info ack
   * corrected wrong parameter index for LATITUDE in list 0
   * answer with NACK if one triggered channel is inhibit
   
** Improvement
   * added two testmode steps to be able to switch the normally opened and the changeover relay directly.
   * added choice for the type of edge for testmode step SERVICE_ID_ZC_DELAY_PREPARE
   * changed testmode zerocrossing measurement pin
   * added inhibit functionality for incoming switch command
   * added lock feature for weekprogram


Version 1.0.2 - 20170330
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469

** Bugfix
   * cyclic status info has no RSSI value of 0x80
   * Actuator remains permanently on after configuration of the changeover time while the actuator is active


Version 1.0.0 - 20170321
--------------------------------------------------------------

** Related Hardware
   * 1554267 + 1724469

** Comments
   * version set to 1.0.0
	 
--- END OF FILE ---
