## [HmIP-SWDO-PL_update_V1_16_10_190227.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SWDO-PL_update_V1_16_10_190227.tgz)
Required CCU firmware version: &#8805; 3.47.10 / 2.47.10<br/>
<sub>sha256: 379e31bf2d9a8b9f7af29a9a2e92f7b553f8a290d84388046da2df69c2f3baac</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version
of the CCUx!

Device: HmIP-SWDO-PL - Homematic IP Window / Door Contact - optical, plus

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 1.16.10 - 20190227
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Added new device type for HmIP-SWDO-PL.
   * Added buildtargets for HmIP-SWDO-PL (similar to HmIP-SWDO-I)

** Comments 
   * 
   

Version 1.16.10 - 20180312
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * [YOU_CTS_OPT_SMI_BN-52][HMIP_SWDO_I-20]Fixed a bug that 
     caused setting of alarmworthy event flag with unidirectional 
     or cyclic status frames.

** Comments
   * 
   
   
Version 1.16.8 - 20180302
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug with receiving answers of conditional switch commands.
   * Also had to correct the counting of sequence counters if 
     they are the same as the sequence counter of the status frame.

** Comments
   * 
   
   
Version 1.16.6 - 20180221
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments
   * Changed counting of event_counter to new mechanism 
     (boot:0; other:[1..252]). [CHANGEMANAGEMENT-483]
	 [YOU_CTS_OPT_SMI_BN-48][HMIP_SWDO_I-19]
   * Reworked the mechanism of receiving answers.
   
   
Version 1.16.4 - 20180209
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Added separate keypress counter for window and backup.
   * All pending flags are now handled after boot process is 
     finished. Otherwise it is possible to miss an acknowledgment  
	 frame of a frame at boot.

** Comments
   *
   
   
Version 1.16.2 - 20180207
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Added first statusinfo to the backup mechanism.

** Comments 
   * 
   
   
Version 1.16.0 - 20180205
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * HMOS 1.20.4
   * Increased version due to creation of a tag.
   
   
Version 1.15.6 - 20180201
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Added mechanism to prevent overwriting of a alarmworthy 
     event with a not alarmworthy one.
	 -> Fast window open and close now also causes a backup.

** Comments 
   * 
   
   
Version 1.15.5 - 20180131
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Excluded cyclic bidi statusinfo from backup mechanism.
	 
	 
Version 1.15.4 - 20180130
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug with missing MAC_ACKs after blinking.
     [YOU_CTS_OPT_SMI_BN-44][HMIP_SWDO_I-17]

** Comments 
   * Added new parameter DISABLE_MSG_TO_AC.
     [YOU_CTS_OPT_SMI_BN-43][HMIP_SWDO_I-16][CHANGEMANAGEMENT-223]
	 
	 
Version 1.15.3 - 20180129
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 'ifdef'-ed some unnecessary parts for contact sensors 
     without optical detection.

** Comments 
   * Added alarm-channel and depending functionality for 
     security solution.
   
   
Version 1.15.2 - 20170803
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed bug in sleep behaviour.
     [YOU_CTS_OPT_SMI_BN-35][CHANGEMANAGEMENT-100]

** Comments 
   * 
   
   
Version 1.15.1 - 20170315
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Update hmos to version 1.19.26
   
   
Version 1.15.0 - 20170315
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
   

Version 1.13.2 - 20161028
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C / 174499A

** Modification
   * add separate sequence counter for status infos

** Bugfix
   * Report link partner problem frame now includes the
      address of the link partner
   * device turn of rx and go to sleep if status info to shc
      was ok but at least one link partner hasn't answered


Version 1.13.1 - 20160425
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug with ACKs to config update request frames.

** Comments 
   * 
   
   
Version 1.13.0 - 20160413
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
   
   
Version 1.11.15 - 20150930
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Small change if the reset procedure gets aborted with a 
     short keypress.
   * Parameter now get loaded on startup to be abble to do the 
     factory reset (local reset needs to be checked).

** Comments 
   * 
	 
	 
Version 1.11.14 - 20150929
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Changed the reset precedure to the new rules.
     (no device functionality and boot blinking during reset, 
	 restart of the device if reset is not done correctly or 
	 gets aborted)
	 
	 
Version 1.11.13 - 20150925
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Changed Full RX timeout between sending start and the 
     callback from ARR-timout to a fix value (1000000) to be 
	 able to check the new router functionality.
   
   
Version 1.11.12 - 20150901
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Added sending of link partner problem frames after 
     not receiving a MAC_ACK.

** Comments 
   *
   
   
Version 1.11.11 - 20150814
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * YOU_CTS_OPT_SMI_BN-29 - The Full RX mode of the trx is 
     retriggered in the tx callback of the conditional switch 
     command.

** Comments 
   *


Version 1.11.10 - 20150805
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug with the current consumption of the BOSCH-TFK.

** Comments 
   *
   
   
Version 1.11.9 - 20150612
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a theoretical bug with the callbacks of the LED module.
     Now the behaviour should be the same as before the change in HMOS.

** Comments 
   * 
   
   
Version 1.11.8 - 20150612
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Made some interface changes due to changes in LIB.
   
   
Version 1.11.7 - 20150528
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added EMC LIB
	 
	 
Version 1.11.6 - 20150528
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Removed APPLICATION_is_TRX_sending function because this 
     function is now provided by the HMOS / Stack with the 
     TRANSCEIVER_is_sending function.
   
   
Version 1.11.5 - 20150520
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Modifications for LIB.
   
   
Version 1.11.4 - 20150511
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added APPLICATION_emc_led_success due to changes in HMOS / Stack.
   
   
Version 1.11.3 - 20150402
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added handling of parameter ENABLE_ROUTING.
   
   
Version 1.11.2 - 20150330
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Corrected a bug with HMIP_MAC_STATUS_OK_ROUTED.

** Comments 
   * 
   
   
Version 1.11.1 - 20150326
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Corrected a bug with the sequence number check.

** Comments 
   * 
   
   
Version 1.11.0 - 20150319
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Increased version due to creation of a tag. 
   
   
Version 1.9.6 - 20150317
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added HMIP_MAC_STATUS_OK_ROUTED to APPLICATION_cb_tx_CndSwCmd. 
   
   
Version 1.9.5 - 20150313
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug that caused sending of an unknown window status 
     after boot if the sabotage switch is pressed.

** Comments 
   * 
   
   
Version 1.9.4 - 20150313
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Fixed a bug with the parameter SAMPLE_INTERVAL that caused
     a deadlock in the device.

** Comments 
   * 
   
   
Version 1.9.3 - 20150311
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Removed define USE_PARTNER due to changes in HMOS / Stack.
   
   
Version 1.9.2 - 20150310
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Removed define ACCEPT_ANY_ROUTER due to changes in HMOS / Stack.
   
   
Version 1.9.1 - 20150309
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Removed some unused ICMP-defines due to changes in HMOS / Stack.
   
   
Version 1.9.0 - 20150302
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Increased Version after creating tag 1.8.0.

** Comments 
   * 
   
   
Version 1.7.3 - 20150220
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Retrigger the event blinking if it was interrupted by config.

** Comments 
   * 
   
   
Version 1.7.2 - 20150219
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * A ConfigUpdateRequest now only gets triggered after a 
     ANSWER_NAK_PEER_UNKNOWN or ANSWER_NAK_INVALID_CHANNEL
	 (old version was a ConfigUpdateRequest after each NACK).

** Comments 
   * 
   
   
Version 1.7.1 - 20150218
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * Corrected the default value for the dutycycle.
   * Corrected handling of ACKs (sequence counter is now also checked).

** Comments 
   * Changed blinksequence during sendattempt to new standard.
   * Added router.c to the project (due to changes in HMOS / Stack).
   
   
Version 1.7.0 - 20150212
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Increased Version after creating tag 1.6.0.
   
   
Version 1.5.2 - 20150210
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added support for parameter SAMPLE_INTERVAL.
   
   
Version 1.5.1 - 20150128
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Added functionality for PCB test of optical sensor.
   
   
Version 1.5.0 - 20150115
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161C

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
	
	
Version 1.3.2 - 20150114
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161A

** Bugfix
   * 

** Comments 
   * Added setting of the inclusion mode
	-> BOSCH: local key only.
	-> eQ3: local and master key.
   
   
Version 1.3.1 - 20150107
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161A

** Bugfix
   * Fixed a bug in calculation / storing of the low_bat_value.

** Comments 
   * 
   
   
Version 1.3.0 - 20141211
--------------------------------------------------------------

** Related Hardware
   * 1343958I / 1454161A

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
	 
	 
Version 1.1.12 - 20141211
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Romoved blinking on dutycycle aswell as prevention of 
     sending if dutycycle is reached.
	 
	 
Version 1.1.11 - 20141211
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Improved blinking after receiving NACKs.
   * Prevent sending of frames if dutycycle is reached. 
     Also start blinking.
	 
	 
Version 1.1.10 - 20141210
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Changed calculation of the parameter DUTY_LIMIT.
   * Moved decoding of the parameter EVENT_DELAYTIME to the 
     set routine of the modulvariable.
   
   
Version 1.1.9 - 20141209
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected some Comments.

** Comments 
   * Added LowBat-Blinking after sending.
   * Changed encoding of the parameter EVENT_DELAYTIME.
   
   
Version 1.1.8 - 20141205
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed average measurement of the battery from the application 
     because this is now done by the HMOS / Stack.
   * Added util.c to the project to calculate average values.
   
   
Version 1.1.7 - 20141203
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Renamed USE_DUTY_CYCLE_LIMIT to USE_APP_DUTY_CYCLE_LIMIT 
     due to changes in HMOS / Stack.
   * Renamed HMIP_APP_set_shc_duty_cycle_limit() to 
     HMIP_APP_set_duty_cycle_limit() due to changes in HMOS / Stack.
   * Renamed HMIP_APP_get_shc_duty_cycle_limit() to 
     HMIP_APP_get_duty_cycle_limit() due to changes in HMOS / Stack.

** Comments 
   * 
   
   
Version 1.1.6 - 20141202
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug in factory reset gesture.

** Comments 
   * 
   
   
Version 1.1.5 - 20141201
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed obsolete include of hal_adc_pre to 
     include of hal.h (including adc.h).

** Comments 
   * 
	 
	 
Version 1.1.4 - 20141201
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added APPLICATION_transceiver_duty_notify due to changes 
     in HMOS / Stack.
   
   
Version 1.1.3 - 20141124
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Fixed a bug in measurement of the battery-voltage during boot.
   
   
Version 1.1.2 - 20141121
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Implemented average measurement of the battery-voltage.
   * Made the gesture of the factory reset more accurate.
   
   
Version 1.1.1 - 20141117
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed HW_CONFIG_CC1100_PATABLE to HW_CONFIG_CC1101_PATABLE 
     due to changes in HMOS / stack.

** Comments 
   * 
   
   
Version 1.1.0 - 20141113
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Increased version number due to creation of a tag.
	 
--- END OF FILE ---