## [HmIP-BSM_update_V1_18_14_200715.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-BSM_update_V1_18_14_200715.tgz)
<sub>sha256: ef3c4d63769bd9338eda047c93118a18da5f106a628dea8c82851c65809b17b4</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:		HmIP-BSM - Switch Actuator and Meter for brand switches

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1 (2 for pluggable).18.14 - 20200715
--------------------------------------------------------------

** Bugfix
   * Made some routines for testing the relay to ram functions. 

** Improvement
   * 

** Comments
   *


Version 1 (2 for pluggable).18.12 - 20200622
--------------------------------------------------------------
** Bugfix
   * After inclusion, device sends bidirectional status telegrams
     to the CCU after approx. 120s


Version 1 (2 for pluggable).18.10 - 20200527
--------------------------------------------------------------

** Bugfix
   * BSM sends Statusframes with ARR every 3 minutes in case that 
     Centrale did not acknowlegeded
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

** Improvement
   * 

** Comments
   *
   
   
Version 1 (2 for pluggable).15.6 - 20190424
--------------------------------------------------------------

** Bugfix
   * SH_PSMR_HMIP-14/CHANGEMANAGEMENT-1148 -
      PowerUpAction is executed although the parameters
      are not yet loaded. 

** Improvement
   * 

** Comments
   *
   
   
Version 1 (2 for pluggable).15.4 - 20190329
--------------------------------------------------------------

** Bugfix
   *  Modify event counter check to meet current specification 

** Improvement
   * 

** Comments
   *
   
   
Version 1 (2 for pluggable).15.2 - 20190308
--------------------------------------------------------------

** Bugfix
   * If the switch-on and switch-off times in the Easy
     Profile are set to "Not active" at the same time, the device hangs up. 

** Improvement
   * 

** Comments
   * Update HMOS to 1.41.58
   
   
Version 1 (2 for pluggable).15.0 - 20190227
--------------------------------------------------------------

** Bugfix
   * FSI16 switches relay to fast if mains power fails (not waiting min
     200 ms) as the the ZCD detection without measuring IC produces IRQs
     only for positive half waves. Timer now has an interval of 20 ms,
     so the relay is switch only if 220 ms has elapsed. 

** Improvement
   * 

** Comments
   * update HMOS to 1.41.45
   
   
Version 1 (2 for pluggable).13.12 - 20181116
--------------------------------------------------------------

** Bugfix
   * Fixed another potentially deadlock.

** Improvement
   * 

** Comments
   * 
   
   
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
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).13.6 - 20180813
--------------------------------------------------------------

** Bugfix
   * Corrected sending of Status-Info 
     frames if the recipent (central or statusinfo receiver)
     is not available.
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).13.4 - 20180628
--------------------------------------------------------------

** Bugfix
   * Corrected bug with weekprogramm 
     at the day of daylight changeover.
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).13.2 - 20180622
--------------------------------------------------------------

** Bugfix
   * Corrected bug with creating direct 
     execution frames in the weekprogramm.
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).13.0 - 20180605
--------------------------------------------------------------

** Bugfix
   * 
	 
** Improvement
   * 
   
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

** Bugfix
   * 
	 
** Improvement
   * 
   
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
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).11.12 - 20180216
--------------------------------------------------------------

** Bugfix
   * Corrected timeout for sequence counter (from 10 to 2 minutes).
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).11.10 - 20180214
--------------------------------------------------------------

** Bugfix
   * Corrected switching direction if switching with current 
     detection is disabled.
	 
** Improvement
   * 
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).11.8 - 20180213
--------------------------------------------------------------

** Bugfix
   * Added sending of unknown RSSI value in two cases.
	 
** Improvement
   * Added new operation mode (minimum HMOS 1.24.0 necessary)
   * Changed counting of event_counter to new mechanism
     (boot:0; other:[1..252]). 
   * Changed checking of event_counter to new mechanism.
        
** Comments 
   * 
  
  
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
	 
** Improvement
   *
   
** Comments 
   * 
   
   
Version 1 (2 for pluggable).11.2 - 20171103
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with sending statusframes with ACK and ARR bit
	 
** Improvement
   *
   
** Comments 
   * 


Version 1 (2 for pluggable).11.0 - 20171013
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with sending statusframes at actuartors 
     with powermeter function.
	 
** Improvement
   *
   
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
   
** Comments 
   
   
Version 1 (2 for pluggable).9.1 - 20170908
--------------------------------------------------------------

** Bugfix

** Improvement
   * new parameter for suppressing messages to Access Controller
   
** Comments 
   * First release version for HmIP-PCBS2


Version 1 (2 for pluggable).8.12 - 20170719
--------------------------------------------------------------

** Bugfix
   * Statusmessage handling corrected

** Improvement
   * Statusmessage handling optimized for multichannel devices
   * No reboot after aborded factory reset
   * new telegrams are only send if previous telegram is acked or timed out
   
** Comments 
   * First release version for HmIP-MOD-OC8
   * Use of bootloader 1.10.0
   
   
Version 1 (2 for pluggable).7.6 - 20170530
--------------------------------------------------------------
 
** Bugfix
   * ARR timeout is not observed 
      with the Info and TimeInformation frames
   * LowBat Bit is not set in the status Info
      
** Improvement
   * DataType Operating Voltage send with StatusInfo
   
** Comments 
   * 
    
    
Version 1 (2 for pluggable).7.5 - 20170519
--------------------------------------------------------------
 
** Bugfix
   * The device reacts with the same 
     event counter for an unconditional switch command.
   * Device is permanently awake.
   
** Comments 
   * 

   
Version 1 (2 for pluggable).7.4 - 20170427
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with not acting device if the 
     channel key was pressed at a included device.

** Comments 
   *
   
   
Version 1 (2 for pluggable).7.3 - 20170426
--------------------------------------------------------------

** Bugfix
   * Increased the power to trigger a simulated 
     keypress from 0.1W to 1 W. 
   * Value for the new powerstatus is saved after 
     being stable for two measurements. 
   * Corrected default duration of weekprogramm to 0xFF.
   * Corrected / Optimised sending of a normal ACK/NACK.

** Comments 
   *
   
   
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


Version 1 (2 for pluggable).5.9 - 20170405
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added new weekprogramm.
   
   
Version 1 (2 for pluggable).5.8 - 20170328
--------------------------------------------------------------

** Bugfix
   * In auto inclusion mode, the triple burst listener device is not a permanent listener.

** Comments 
   * 
   
   
Version 1 (2 for pluggable).5.7 - 20170308
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with the sequence counter in the unicast frame 
     (for collecting ACKs) after sending multicast frames due 
	 to a long keypress.

** Comments 
   * 
   
   
Version 1 (2 for pluggable).5.0 - 20161209
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
   
   
Version 1 (2 for pluggable).3.8 - 20161128
--------------------------------------------------------------

** Bugfix
   * Corrected a bug with RSSI calculation in statusInfo.

** Comments 
   * 
   
   
Version 1 (2 for pluggable).3.7 - 20161114
--------------------------------------------------------------

** Bugfix
   * Fixed a bug that caused errors with one partner linked 
     to more channels.

** Comments 
   * 
   
   
Version 1 (2 for pluggable).3.6 - 20161104
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with sending unrequested ACKs.

** Comments 
   * 
   
   
Version 1 (2 for pluggable).3.5 - 20161021
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added switching the relay as EMC action.
   
   
Version 1 (2 for pluggable).3.4 - 20160926
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with the simulated keypress generated from 
     the powermeter task.

** Comments 
   *


Version 1 (2 for pluggable).3.3 - 20160913
--------------------------------------------------------------

** Bugfix
   * Added IDLE state to switch task.
   * Corrected behaviour of the powerfailure function.
   * Corrected behaviour of the overhead function.
   * Suppressed sending of StatusInfoFrames if the device is 
     not included.
   * Corrected behaviour of factory reset if the keyVisual is 
     pressed during powerUp.

** Comments 
   *
   
   
Version 1 (2 for pluggable).3.2 - 20160901
--------------------------------------------------------------

** Bugfix
   * Included hmos 1.16.2 which fixed a bug with exlusion after inclusion

** Comments 
   *
   

Version 1 (2 for pluggable).3.1 - 20160721
--------------------------------------------------------------

** Bugfix
   * Corrected size of action type.
   * Fixed a bug that caused not spawning conditional switch 
     channel task.
   * Fixed setting of the decision value for falling direction 
     in the conditional switch channel.

** Comments 
   *
   
   
Version 1 (2 for pluggable).3.0 - 20160719
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
   
   
Version 1 (2 for pluggable).1.17 - 20160718
--------------------------------------------------------------

** Bugfix
   * StutusInfo frames from the switch module can now be send 
     with ARR-Bit. 
     StatusInfo frames from the powermeter are still 
     unidirectional all the time.

** Comments 
   * 
	 
	 
Version 1 (2 for pluggable).1.16 - 20160714
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Removed sending of config update requests on buttonpress 
     of the keyvisual for all permanent powered actuators.
   
   
Version 1 (2 for pluggable).1.15 - 20160708
--------------------------------------------------------------

** Bugfix
   * Fixed bug that first reset step is ready before 
     the timeout of 4 seconds occur.
   * Suppress boot blinking if reset is in progress.
   * Fixed a bug with index of parameter arrays if the key 
     visual is used as channel key. 

** Comments 
   * 
	 
	 
Version 1 (2 for pluggable).1.14 - 20160704
--------------------------------------------------------------

** Bugfix
   * Conditional switch channel gets now removed in idle state.

** Comments 
   * Set the default values for event delay of output1, 
     meter and conditional channel from 1 to 3 seconds.
   * Powermeter arrays for averaging now always get resetted 
     if SWITCH_set_level_real() is called.
	 
	 
Version 1 (2 for pluggable).1.13 - 20160616
--------------------------------------------------------------

** Bugfix
   * Fixed a bug in evaluation of long keypresses 
     for the pairing mode.
   * Fixed a bug with setting parameters for the 
     input channel.

** Comments 
   * Set default value for the longpress time in the 
     HmIP-PSx devices to 4s.
   
   
Version 1 (2 for pluggable).1.12 - 20160613
--------------------------------------------------------------

** Bugfix
   * Corrected some typos.

** Comments 
   * Added conditional switch channel.
	 
	 
Version 1 (2 for pluggable).1.11 - 20160531
--------------------------------------------------------------

** Bugfix
   * Reset ACCEPT_ANY_DEVICE to 0.

** Comments 
   * Major version increased to 2.
     Minor and Path number will run parallel for all devices.
	 
	 
Version 1.1.10 - 20160518
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added routines for HmIP-PS.
   * Renamed CS5490_zc.c /.h to zerocrossing_interrupt.c / .h 
     to be more general.
   * Smaller changes to the DUMMY_SGTIN.
   * Reduced number of partners for HmIP-PSx to 20. 
     With this all switch actuators act the same.
	 
	 
Version 1.1.9 - 20160512
--------------------------------------------------------------

** Bugfix
   * Corrected a bug with the switching direction.

** Comments 
   * Added visualisation of the channelstate with the key 
     visual (Including the parameter) to all actuators. 
   
   
Version 1.1.8 - 20160510
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added pairing functionality.
   
   
Version 1.1.7 - 20160509
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added routing functionality.
   
   
Version 1.1.6 - 20160509
--------------------------------------------------------------

** Bugfix
   * Some style changes.
   * Corrected calculation of energycount.

** Comments 
   * Some optimisations on startup.
	 
	 
Version 1.1.5 - 20160503
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Corrected some comments and function headers.
   * Corrected parameter for energy threshold. It was one byte 
     but has to be two byte.
   * Added parameter LED_DISABLE in list1 of the 
     real channel.
	 
	 
Version 1.1.4 - 20160502
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added default link between key visual and 
     the switch channel.
   * Added routines to do visialisation of the 
     channel state with the key visual.
   * Corrected factory reset gesture 
     (only valid at power up).
   
   
Version 1.1.3 - 20160428
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Added key routines for switching with the key visual.
   
   
Version 1.1.2 - 20160426
--------------------------------------------------------------

** Bugfix
   * Fixed to which multicast addresses the device listens.

** Comments 
   * Startet porting code to the PSM hardware.
   
   
Version 1.1.1 - 20160425
--------------------------------------------------------------

** Bugfix
   * Fixed a bug with ACKs to config update request frames.

** Comments 
   *
   
   
Version 1.1.0 - 20160413
--------------------------------------------------------------

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
	 
	 
--- END OF FILE ---