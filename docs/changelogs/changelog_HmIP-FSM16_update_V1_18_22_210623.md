## [HmIP-FSM16_update_V1_18_22_210623.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-FSM16_update_V1_18_22_210623.tgz)
<sub>sha256: f3af3acfafd2a7dc33e3a810287c697b21757ed0f5fd94ea93c03f16482fe69d</sub>
Required CCU firmware version: &#8805; 3.41.9 / 2.41.9

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!
             If the switching actuator is operated in two-point control and the firmware version is 1.18.14, 
             we recommend to remove the batteries from the wall thermostat until the actuator update has been 
             successfully done. Otherwise the transmission of the firmware will be interrupted.

Device:	     HmIP-FSM16 - Switch Actuator and Meter (16 A) - flush mount

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1 (2 for pluggable).18.22 - 20210412
--------------------------------------------------------------
** Bugfix
   * Device responds on multicast frames without ARR bit
   * Device sends Status-Frames with Ack-Flag on SwichCommands without ARR-Flag


Version 1 (2 for pluggable).18.20 - 20210115
--------------------------------------------------------------
** Bugfix
   * Fixed a bug that with not removing calibration task.
   
   
Version 1 (2 for pluggable).18.18 - 20210106
--------------------------------------------------------------
** Improvement
   * Switched to usage of internal OSC with permanent calibraton 
     from the HFXO due to problems when switching non omic loads.
     
   
Version 1 (2 for pluggable).18.16 - 20200803
--------------------------------------------------------------
** Bugfix
   * Added missing defines for the new statusinfo module in PS, 
     thus also in PCBS.

 
Version 1 (2 for pluggable).18.14 - 20200715/20200710
--------------------------------------------------------------
** Bugfix
   * Move some routines for testing the relay to ram functions. 
   * Device send status continuously and leads CCU and device running into duty cycle


Version 1 (2 for pluggable).18.12 - 20200622
--------------------------------------------------------------
** Bugfix
   * After inclusion, device sends bidirectional status telegrams
     to the CCU after approx. 120s


Version 1 (2 for pluggable).18.10 - 20200527
--------------------------------------------------------------
** Bugfix
   * BSM sends Statusframes with ARR every 3 minutes in case that SHC did not acknowlegeded
   * RSSI-value in AnswerFrame always 0dBm
   * BSM does not respond to a keystroke if a switching command was previously
     received on the actuator channel from an unknown link partner
     
** Modification
   * Update to HMOS 1.46.1


Version 1 (2 for pluggable).18.6 - 20200309
--------------------------------------------------------------
** Bugfix
   * Device sends answers-frame on a TimeInfo from AC to "any-router"-address
   * Device sends ack frames if ARR bit is not set


Version 1 (2 for pluggable).18.4 - 20200226
--------------------------------------------------------------
** Bugfix
   * Channel keys without function if external link partner could not be reached and DisableMSGToAC = true
   * Device sends status info with "Level with profile Information" instead of "Binary with profile Information"
   * Parameter DisableMSGtoAC without function if multicast address is set as system partner
   * If the button is pressed to fast after restart, the device does not switch permanently any more.	
     
     
Version 1 (2 for pluggable).18.2 - 20200212
--------------------------------------------------------------
** Bugfix
   * Device running into duty cycle if CCU or HAP is not available
   * Update status info sending rules
   * Configuration is not longer shown on LED, if a key is pressed while getting config data

** New Feature
   * Using status info module
   
   
Version 1 (2 for pluggable).16.0 - 20191121
--------------------------------------------------------------
** Bugfix
   * If possible, send multicasts only to PARTNER_ALL_WIRED_DEVICES instead of to PARTNER_ALL_DEVICES.
   * Device reboots if relay has to be switched
   * fixed bug in device behavior, if message to ac is disabled
   * fixed bug if factory reset is aborted
   * Fixed a bug in the zero crossing module due to new version of emlib

** Modification
   * Update HMOS to 1.44.2
   * Update Bootloader to 1.14 (Fixed inverted LEDs in bootloader in V1.14.2)
   * Modify emlib makro calls due to changes in updated emlib

** New Feature
   * Support of HmIP-FSI16
   * Add support for switch inputs
   * Add relay count feature


Version 1 (2 for pluggable).14.4 -20190424 (Hotfix)
--------------------------------------------------------------
** Bugfix
   * PowerUpAction is executed although the parameters are not yet loaded.
   * If the switch-on and switch-off times in the Easy Profile are set to "Not active" at the same time, the device hangs up.
   * Modify event counter check to meet current specification


Version 1 (2 for pluggable).14.2 -20190311
--------------------------------------------------------------
** Bugfix
   * Modify event counter check to meet current specification
   * If the switch-on and switch-off times in the Easy Profile are set to "Not active" at the same time, the device hangs up. 
   * FSI16 switches relay to fast if mains power fails (not waiting min 200 ms) as the the ZCD detection without measuring IC produces IRQs
     only for positive half waves. Timer now has an interval of 20 ms, so the relay is switch only if 220 ms has elapsed. 


Version 1 (2 for pluggable).14.0 - 20181212
--------------------------------------------------------------
** Bugfix
   * PSMR/PSM doesn't switch if the key visual is pressed directly after the boot process is finished (green led signal)
   * Corrected sending of Status-Info frames if the recipent (central or statusinfo receiver) is not available.
   * Stopped sending inclusion request on each long keypress repetition
   * Fixed another potentially deadlock.
   * Race condition may cause deadlock
   * Corrected bug with weekprogramm at the day of daylight changeover.
   * Corrected bug with creating direct execution frames in the weekprogramm.

** Improvement
   * check of keypress counter and application sequence counter updated   
   

Version 1 (2 for pluggable).12.6 - 20181119 (Hotfix)
--------------------------------------------------------------
** Bugfix
   * Corrected sending of Status-Info frames if the recipent (central or statusinfo receiver) is not available.   
   * Stopped sending inclusion request on each long keypress repetition.   
   * Race condition may cause deadlock 
   * Fixed another potentially deadlock.
	 
** Improvement
   * check of keypress counter and application sequence counter updated
   
** Comments 
   * Update HMOS to 1.36.0
   
   
Version 1 (2 for pluggable).12.4 - 20180628 (Hotfix)
--------------------------------------------------------------
** Bugfix
   * Corrected bug with weekprogramm at the day of daylight changeover.
   
   
Version 1 (2 for pluggable).12.2 - 20180622 (Hotfix)
--------------------------------------------------------------
** Bugfix
   * Corrected bug with creating direct execution frames in the weekprogramm.
   
   
Version 1 (2 for pluggable).12.0 - 20180605
--------------------------------------------------------------
** Bugfix
   * Increased HMOS version to 1.30.0 to be able to route inclusion frames (with routing actuators).
	 
** Improvement
   * Added functionality and configuration parameters to do "OFF-Actions" at powerup.

     
** Comments
   

Version 1 (2 for pluggable).10.14 - 20180313
--------------------------------------------------------------
** Comments 
   * Changed default value for the long keypress from 4s to 0,4s. Necessary modifications to leave the pairing function as it is.
   
   
Version 1 (2 for pluggable).10.12 - 20180226
--------------------------------------------------------------
** Bugfix
   * Added reset of measurement array after switching to prevent next measurement to be outdated. An outdated array may cause wrong switching!


Version 1 (2 for pluggable).10.10 - 20180220
--------------------------------------------------------------
** Bugfix
   * Fixed wrong reset of a pending flag if disable_msg_to_ac was set.
   * Added sending of unknown RSSI value in two cases.
   * Corrected switching direction if switching with current detection is disabled.
   * Corrected timeout for sequence counter (from 10 to 2 minutes).
   
** Comments 
   * Changed default value for POWERUP_ONTIME from 0x00 to 0xFF.
   * Added new operation mode (minimum HMOS 1.24.0 necessary)
   * Changed counting of event_counter to new mechanism (boot:0; other:[1..252])
   * Changed checking of event_counter to new mechanism.
   
   
Version 1 (2 for pluggable).10.8 - 20171222
--------------------------------------------------------------
** Bugfix
   * Fixed bug with fast switching
   
   
Version 1 (2 for pluggable).10.6 - 20171106
--------------------------------------------------------------
** Bugfix
   * Fixed a bug with sending statusframes with ACK and ARR bit


Version 1 (2 for pluggable).10.4 - 20171020
--------------------------------------------------------------
** Bugfix
   * Fixed a bug with sending statusframes at actuartors
     with powermeter function.
   
   
Version 1 (2 for pluggable).10.2 - 20171009
--------------------------------------------------------------
** Comments 
   * Increased version of HMOS to 1.20.4.
   
   
Version 1 (2 for pluggable).10.0 - 20171006
--------------------------------------------------------------
** Bugfix
   * Corrected behaviour of weekprogrammm for neagtive coordiantes.
   * Changed behaviour of init routines in powermeter- and switch-task.
   * Fixed behaviour of sending statusmessages for multichannel devices. 
   
** Improvement
   * new parameter for suppressing messages to Access Controller

--- END OF FILE ---