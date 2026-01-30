## [HmIP-FSM_update_V1_18_22_210623.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-FSM_update_V1_18_22_210623.tgz)
<sub>sha256: 9be4afad7c52b50b451e4185b3388b59379a761e28ad432d80f06f582e9183d1</sub>
Required CCU firmware version: &#8805; 3.41.9 / 2.41.9

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!
             If the switching actuator is operated in two-point control and the firmware version is 1.18.14, 
             we recommend to remove the batteries from the wall thermostat until the actuator update has been 
             successfully done. Otherwise the transmission of the firmware will be interrupted.

Device:		HmIP-FSM - Switch Actuator and Meter - flush mount

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany


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

   
Version 1 (2 for pluggable).18.14 - 20200715
--------------------------------------------------------------
** Bugfix
   * Made some routines for testing the relay to ram functions. 


Version 1 (2 for pluggable).18.12 - 20200622
--------------------------------------------------------------
** Bugfix
   * After inclusion, device sends bidirectional status telegrams
     to the CCU after approx. 120s


Version 1 (2 for pluggable).18.10 - 20200527
--------------------------------------------------------------
** Bugfix
   * BSM sends Statusframes with ARR every 3 minutes in case that 
     SHC did not acknowlegeded
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
   * Channel keys without function if external link
     partner could not be reached and DisableMSGToAC = true
   * Device sends status info with "Level with profile Information" 
     instead of "Binary with profile Information"
   * Parameter DisableMSGtoAC without function
     if multicast address is set as system partner
   * If the button is pressed to fast after restart ,
     the device does not switch permanently any more.	
     

Version 1 (2 for pluggable).18.2 - 20200212
--------------------------------------------------------------
** Bugfix
   * Device running into duty cycle if CCU or HAP is not available
   * Update status info sending rules
   * Configuration is not longer shown on LED, 
     if a key is pressed while getting config data

** New Feature
   * Using status info module
   

Version 1 (2 for pluggable).16.0 - 20191121
--------------------------------------------------------------
** Bugfix
   * Fixed inverted LEDs in bootloader (V1.14.2)

** Modification
   * Update HMOS to 1.44.2

** New Feature
   * Support of HmIP-FSI16


Version 1 (2 for pluggable).15.10 to 15.24 - 20191106 
--------------------------------------------------------------
** Bugfix
   * If possible, send multicasts only to PARTNER_ALL_WIRED_DEVICES
     instead of to PARTNER_ALL_DEVICES.
   * Device reboots if relay has to be switched
   * fixed bug in device behavior, if message to ac is disabled
   * fixed bug if factory reset is aborted
** Modification
   * Modify emlib makro calls due to changes in updated emlib
   * Update HMOS to 1.43.41
   * Update Bootloader to 1.14

** New Feature
   * Add support for switch inputs
   * Add relay count feature
   

Version 1 (2 for pluggable).15.8 - 20190522
--------------------------------------------------------------
** Bugfix
   * Fixed a bug in the zero crossing module due to new 
     version of emlib. 

   
Version 1 (2 for pluggable).15.6 - 20190424
--------------------------------------------------------------
** Bugfix
   * PowerUpAction is executed although the parameters
      are not yet loaded. 
 
   
Version 1 (2 for pluggable).15.4 - 20190329
--------------------------------------------------------------
** Bugfix
   * Modify event counter check to meet current specification 

   
Version 1 (2 for pluggable).15.2 - 20190308
--------------------------------------------------------------
** Bugfix
   * If the switch-on and switch-off times in the Easy
     Profile are set to "Not active" at the same time, the device hangs up. 

** Comments
   * Update HMOS to 1.41.58
   
   
Version 1 (2 for pluggable).15.0 - 20190227
--------------------------------------------------------------
** Bugfix
   * FSI16 switches relay to fast if mains power fails (not waiting min
     200 ms) as the the ZCD detection without measuring IC produces IRQs
     only for positive half waves. Timer now has an interval of 20 ms,
     so the relay is switch only if 220 ms has elapsed. 

** Comments
   * update HMOS to 1.41.45
   
   
Version 1 (2 for pluggable).13.12 - 20181116
--------------------------------------------------------------
** Bugfix
   * Fixed another potentially deadlock.

  
   
Version 1 (2 for pluggable).13.10 - 20181115
--------------------------------------------------------------
** Bugfix
   * Race condition may cause deadlock

** Improvement
   * check of keypress counter and application sequence counter updated

** Comments
   * Update HMOS to 1.39.1
   
   
Version 1 (2 for pluggable).13.8 - 20181026
--------------------------------------------------------------
** Bugfix
   * Stopped sending inclusion request on each long keypress 
     repetition.
	 
   
Version 1 (2 for pluggable).13.6 - 20180813
--------------------------------------------------------------
** Bugfix
   * Corrected sending of Status-Info 
     frames if the recipent (central or statusinfo receiver)
     is not available.
  
   
Version 1 (2 for pluggable).13.4 - 20180628
--------------------------------------------------------------
** Bugfix
   * Corrected bug with weekprogramm 
     at the day of daylight changeover.
	 
   
Version 1 (2 for pluggable).13.2 - 20180622
--------------------------------------------------------------
** Bugfix
   * Corrected bug with creating direct 
     execution frames in the weekprogramm.
  
   
Version 1 (2 for pluggable).13.0 - 20180605
--------------------------------------------------------------
** Comments 
   * Increased version number due to creation of a tag.


Version 1 (2 for pluggable).11.17 - 20180601
--------------------------------------------------------------
** Bugfix
   * Increased HMOS version to 1.30.0 to be able to route 
     inclusion frames (with routing actuators).
	 
** Improvement
   * Added functionality and configuration 
     parameters to do "OFF-Actions" at powerup.
   
** Comments 
	 
	 
Version 1 (2 for pluggable).11.16 - 20180309
--------------------------------------------------------------
** Comments 
   * Changed the default 
     value for the long keypress from 4s to 0,4s. Did necessary 
     modifications to leave the pairing function as it is.
   
   
Version 1 (2 for pluggable).11.14 - 20180223
--------------------------------------------------------------
** Bugfix
   * Added reset of measurement array after switching 
     to prevent next measurement to be outdated. An outdated 
     array may cause wrong switching!
   
   
Version 1 (2 for pluggable).11.12 - 20180216
--------------------------------------------------------------
** Bugfix
   * Corrected timeout for sequence counter (from 10 to 2 minutes).
	 
   
Version 1 (2 for pluggable).11.10 - 20180214
--------------------------------------------------------------
** Bugfix
   * Corrected switching direction if switching with current 
     detection is disabled.
  
   
Version 1 (2 for pluggable).11.8 - 20180213
--------------------------------------------------------------
** Bugfix
   * Added sending of unknown RSSI value in two cases.
	 
** Improvement
   * Added new operation mode (minimum HMOS 1.24.0 necessary)
   * Changed counting of event_counter to new mechanism
     (boot:0; other:[1..252]).
   * Changed checking of event_counter to new mechanism.

  
Version 1 (2 for pluggable).11.6 - 20180205
--------------------------------------------------------------
** Bugfix
   * Fixed wrong reset of a pending flag if disable_msg_to_ac was set.
	 
** Improvement
   * Corrected some comments.
   
** Comments 
* Changed default value for POWERUP_ONTIME from 0x00 to 0xFF.
   
   
Version 1 (2 for pluggable).11.4 - 20171219
--------------------------------------------------------------
** Bugfix
   * Fixed bug with fast switching
	 
   
Version 1 (2 for pluggable).11.2 - 20171103
--------------------------------------------------------------
** Bugfix
   * Fixed a bug with sending statusframes with ACK and ARR bit
	 

Version 1 (2 for pluggable).11.0 - 20171013
--------------------------------------------------------------
** Bugfix
   * Fixed a bug with sending statusframes at actuartors 
     with powermeter function.
	 
** Comments 
   * Increased version number due to creation of a tag.


Version 1 (2 for pluggable).9.2 - 20171006
--------------------------------------------------------------
** Bugfix
   * Corrected behaviour of weekprogrammm for neagtive coordiantes.
   * Changed behaviour of init routines in powermeter- and switch-task.
   * Fixed behaviour of sending statusmessages 
     for multichannel devices. 
	 
** Improvement
   
   
Version 1 (2 for pluggable).9.1 - 20170908
--------------------------------------------------------------
** Improvement
   * new parameter for suppressing messages to Access Controller
   

Version 1 (2 for pluggable).8.12 - 20170719
--------------------------------------------------------------
** Bugfix
   * Statusmessage handling corrected

** Improvement
   * Statusmessage handling optimized for multichannel devices
   * No reboot after aborded factory reset
   * new telegrams are only send if previous telegram is acked or timed out
   
** Comments 
   * Use of bootloader 1.10.0
   
   
Version 1 (2 for pluggable).7.6 - 20170530
--------------------------------------------------------------
** Bugfix
   * ARR timeout is not observed 
      with the Info and TimeInformation frames
   * LowBat Bit is not set in the status Info
      
** Improvement
   * DataType Operating Voltage send with StatusInfo
 

Version 1 (2 for pluggable).7.5 - 20170519
--------------------------------------------------------------
** Bugfix
   * The device reacts with the same 
     event counter for an unconditional switch command.
   * Device is permanently awake.
   
  
Version 1 (2 for pluggable).7.4 - 20170427
--------------------------------------------------------------
** Bugfix
   * Fixed a bug with not acting device if the 
     channel key was pressed at a included device.


Version 1 (2 for pluggable).7.3 - 20170426
--------------------------------------------------------------
** Bugfix
   * Increased the power to trigger a simulated 
     keypress from 0.1W to 1 W.
   * Value for the new powerstatus is saved after 
     being stable for two measurements.
   * Corrected default duration of weekprogramm to 0xFF.
   * Corrected / Optimised sending of a normal ACK/NACK.

Version 1 (2 for pluggable).7.2 - 20170425
--------------------------------------------------------------
** Bugfix

** Comments 
   * Removed ramp time from the weekprogram.
   * Added sending of statusframes for the weekprogram.
     (After inclusion, cyclic and on request)
   * Corrected a bug with inhibit channels.
	  
	  
Version 1 (2 for pluggable).7.1 - 20170413
--------------------------------------------------------------
** Bugfix

** Comments 
   * Added lock feature to weekprogramm channel.
   * Added delayed weekprogram status info to status info
      receiver after change of lock channels.
   
   
Version 1 (2 for pluggable).7.0 - 20170405
--------------------------------------------------------------
** Bugfix
   * Increased the pulse for switching the relais 
     from 30 ms to 75 ms.

** Comments 
   * Increased version due to creation of a tag.


--- END OF FILE ---