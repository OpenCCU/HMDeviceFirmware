## [HmIP-SWDO-I_update_V1_16_10_180314.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SWDO-I_update_V1_16_10_180314.tgz)
<sub>sha256: 60eb34f0ee3ac04b5af290dbd75c9fec79bb97acc56e7e7ca6e939cb85eb797c</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.33.3

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der aktuellsten CCU2/3 Version.

Please note: Only use the firmware file in connection with the latest CCU2/3 version.


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
	 
	 
Version 0.8.10 - 20141113
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added workaround to prevent mearuring with the IR-diode 
     while sending with the TRX-module.
   
   
Version 0.8.9 - 20141112
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Corrected IO-Port (LBT-mentioning) of TRX module.
	 
	 
Version 0.8.8 - 20141112
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed clearing of the LEDs before going to power down 
     due to changes in HMOS / Stack.
   * Removed POWER_prepare_powerdown() from application due 
     to changes in HMOS / Stack.
   * Made some improvements in the getter and setter functions 
     for the low-bat-limit-parameter.
   
   
Version 0.8.7 - 20141112
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected a bug that caused no sending of StatusInfo 
     frames if any part of the receiver address is 0x00.

** Comments 
   * 
	 
	 
Version 0.8.6 - 20141111
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed switching of the inclusion mode because the HMOS 
     now has LocalKey and MasterKey as default.
   * Removed setting of the Teststatus on startUp because this 
     is not longer supported by the HMOS.
   * Made some small changed to prepare a saver Power down on 
     very low bat.
   
   
Version 0.8.5 - 20141110
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed workaround with delayed StatusInfo after inclusion.

** Comments 
   * 
	 
	 
Version 0.8.4 - 20141107
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added callback status to the inclusion callback due to 
     changes in HMOS / Stack.
   
   
Version 0.8.3 - 20141106
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug that caused wrong blinking if the StatusInfo 
     receiver was set to 0x000000.

** Comments 
   * Added new mechanism to measure the batteries due to 
     changes in HMOS / Stack.
   * Added 0x7FF to the first timer of the StatusInfo to make 
     sure it is send after the first inclusion request / 
	 nighborhood advertisement. This ensures a valid value 
	 of the batterie voltage for the StatusInfo.
   * Removed build-target for FULL_RX because it is not longer 
     used.
   * Removed some unused and obsolete code.
   
   
Version 0.8.2 - 20141105
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Put #ifdefs arount the sabotage-contact funtionality 
     because only the optic version has this switch.

** Comments 
   * 
   
   
Version 0.8.1 - 20141104
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed default value of LIST0_CYCLIC_INFO_MSG_DIS for 
     the BOSCH-device to 0x00.

** Comments 
   * Added checking of StatusInfo with ACK-bit in rx-callback.
   
   
Version 0.8.0 - 20141031
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Incremented version after new TAG.
   * Added m_full_rx_node_application due to changes in HMOS / Stack.
	 
	 
Version 0.7.1 - 20141031
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Moved registration of the callback for the keys back in 
     the init routine because it caused misbehaviour in HMOS.

** Comments 
   * Removed unnecessary initialisation of System-Key-3 
     (REED contact) from the init.
   * Made the sensor detection more robust. -> prevent sending 
     of frames on BOOT.
   
   
Version 0.7.0 - 20141030
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Device now checks the status of the window sensor on startup.

** Comments 
   * 
   
   
Version 0.6.11 - 20141030
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * APPLICATION_get_m_window_status() now returns the correct 
     type (ir_sensor_status_t).

** Comments 
   * Reduced speed of the I2C to 100 KHz.
   
   
Version 0.6.10 - 20141029
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Moved registration of the callback for the keys behind the 
     boot blinking so that the pulled up capacitors have enough 
	 time to settle.

** Comments 
   *
   
   
Version 0.6.9 - 20141028
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Timer callback now stops sending of inclusion requests 
     if the device has been service included.
   * Corrected some issues with execute- and report-teststep 
     due to changes in the application protocol.

** Comments 
   * 
	 
	 
Version 0.6.8 - 20141027
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Changed return-value of APPLICATION_cb_rx() from void to 
     RETURN_status_t due to HMOS / Stack changes.
   
   
Version 0.6.7 - 20141027
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added service inclusion to the device.
   * Removed dummy pin.
	 
	 
Version 0.6.6 - 20141023
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added APPLICATION_config_show() and its callback to the 
     application due to changes in HMOS / Stack.
   
   
Version 0.6.5 - 20141022
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug that cause sending of multiple StatusInfo 
     frames on startUp.

** Comments 
   * 
   
   
Version 0.6.4 - 20141022
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * The BiDi StatusInfo that is send once per hour to once 
     per day now only gets send if the device is included.

** Comments 
   * 
	 
	 
Version 0.6.3 - 20141022
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added USE_HMIP_CYCLIC_TX and USE_HMIP_CYCLIC_RX due to 
     changes in HMOS / Stack.
   
   
Version 0.6.2 - 20141021
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added checking of the return value of 
     HMIP_NETMGMT_is_included due to changes in HMOS / Stack.
   * Added sending of a StatusInfo on Boot.
   
   
Version 0.6.1 - 20141017
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Prevent sending of a ConfigUpdateRequest if the AC is 
     not reachable.

** Comments 
   * 
	 
	 
Version 0.6.0 - 20141017
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed StatusInfo-Receiver from parameterlists 
     (not longer supported by HMOS).
   
   
Version 0.5.8 - 20141016
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New versin number to test the Update functionality.
   
   
Version 0.5.7 - 20141016
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug that caused no sending of the first StatusInfo 
     after inclusion.

** Comments 
   * 
   
   
Version 0.5.6 - 20141015
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Now the device doesn't goto full rx after sending a 
     unidirectional StatusInfo.

** Comments 
   * 
   
   
Version 0.5.5 - 20141015
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug in StatusInfo and CndSwCmd when MSG_FOR_POS_X 
     was set to 0 (no message shall be send)

** Comments 
   * Corrected some errors / typos dou to doxygen doku.
   
   
Version 0.5.4 - 20141013
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed a bug in battery-measurement.

** Comments 
   * 
	 
	 
Version 0.5.3 - 20141010
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added APPLICATION_emc_led() and APPLICATION_emc_action()
     to the application due to changes in HMOS / Stack.
   
   
Version 0.5.2 - 20141009
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed useless and obsolete defines.
   * Changed EMV_MODE to EMC_MODE due to actualisation of 
     the HMOS / Stack.

** Comments 
   * 
   
   
Version 0.5.1 - 20141002
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Made some changes due to changes in HMOS / Stack.

** Comments 
   * 
   
   
Version 0.5.0 - 20141002
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Added names to the application.c and application.h file 
     header.
   * Corrected some typos in comments.
   * Added include to frames.h.
   * Changes some defines in config.h during changes in 
     HMOS / Stack.

** Comments 
   * Added Testmode for production to the device.
   * Removed hal_CC1100.c, hal_Si4431.c, CC1100.c and Si4431.c.
   * Added transceiver_CC1101.c due to changes in HMOS / Stack.
   * Some changes in config files due to changes in HMOS / Stack.
	 
	 
Version 0.4.4 - 20140925
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Each 30 pseudo-cyclic intervall will now trigger a 
     bidi StatusInfo (approx. each hour).
   * The SatusInfo-Telegramm now won't be send if the 
     StatusInfo-Receiver is set to 0x000000.
   
   
Version 0.4.3 - 20140925
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Changed green blinking at factory reset.
   
   
Version 0.4.2 - 20140925
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Now the Application-Task is just spawned if the 
     cyclic-StatusInfo really needs to be send.
   * Removed unecessary comment.

** Comments 
   * 
   
   
Version 0.4.1 - 20140919
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Replaced m_sequence_number_statusinfo with m_sequence_number
	 in the StatusInfo-Telegramm.

** Comments 
   * 
	 
	 
Version 0.4.0 - 20140918
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed ACCEPT_ALL_MAINS_POWERED_DEVICES from config.h 
     because the shutter contact shall not listen to such frames.

** Comments 
   * Added Timeout to the function TRANSCEIVER_goto_full_rx.
     -> necessary due to HMOS / Stack changes.
	 
	 
Version 0.3.9 - 20140916
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * The LED now flashes green if the StatusInfo due to an Event
     was send to an ANY or ALL address.

** Comments 
   * Removed some unnecessary warnings.
   * Added red blink code if the user trys to factory reset the
     device with the button wich is locked by the configuration.
   * Added red blink code if the user makes the wrong gesture 
     on factory reset.
	 
	 
Version 0.3.8 - 20140910
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Added blink sequence on startUp.

** Comments 
   * Removed some unnecessary parameters from the send callbacks.
     -> change in HMOS / Stack.
   
   
Version 0.3.7 - 20140909
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Restart of auto-inclusion after change of the window status 
     only if factory reset is not active.

** Comments 
   * Increased ICMP intervall from 10 minutes to 1 hour.
   * Added compiler-switch to turn on FULL_RX-mode.
   
   
Version 0.3.6 - 20140814
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed unnecessary checking of application frametype from 
     rx callback. (Forgotten in Version 0.3.3)
   * Removed unnecessary declaration.

** Comments 
   * Added enum for the factory reset states.
   
   
Version 0.3.5 - 20140813
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New version of HMOS (release 91372).
   
   
Version 0.3.4 - 20140813
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Added initialisation of the send options for ConfigUpdateRequest.

** Comments 
   * 
	 
	 
Version 0.3.3 - 20140811
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New version of HMOS (release 91316).
   * Removed workaround to filter all not application frames 
     because this is done by the stack now.
	 
	 
Version 0.3.2 - 20140811
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added workaround to send with full send power.
   * Added workaround to filter all frames except application 
     frames in callback. So the callback only has to check 
	 these application frames.
	 
	 
Version 0.3.1 - 20140808
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * If not all frames of an event have been ACKed the device 
     sends a ConfigUpdateRequest.
	 
	 
Version 0.3.0 - 20140808
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * The ConfigUpdateRequest is not longer send when the 
     StatusInfo receiver doesn't differ from the SNC.
   
   
Version 0.2.13 - 20140808
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected default values for CYCLIC_INFO_MSG_DIS and 
     CYCLIC_INFO_MSG_DIS_UNCHANGED

** Comments 
   * New version of HMOS (release 91238).
	 
	 
Version 0.2.12 - 20140807
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Improved blink-sequence of events.
   * Fixed a bug (blinking first code after second blinkcode 
     has already occured) in factory reset blink sequence. 
   * Fixed a bug that the first StatusInfo telegramm has to 
     be ACKed.

** Comments 
   * New version of HMOS (release 91211).
   * Device now has inclusion mode MasterKey AND LocalKey as 
     default. This is not longer switchable with the key!
   * Removed setting of the including AC as StatusInfo receiver 
     because this caused a bug with the MAC sequence number 
	 validation. 
	 Setting of the StatusInfo receiver is now done by HMOS 
	 during inclusion process.
	 
	 
Version 0.2.11 - 20140804
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Moved marking that the CndSwCmd and the StatusInfo needs to 
     be acked after EventDelay instead after each callback to 
	 avoid multiple blinking.

** Comments 
   * Added DutyCycle flag for 868MHz in StatusInfo.
   * Added mechanism to send the first StatusInfo after inclusion 
     with 2s delay to avoid a collision with mac sequence number 
	 validation.
   * Added blinking orange after EventDelay to signalise 
     following send attempt.
   
   
Version 0.2.10 - 20140801
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed some comments.
   * Fixed a bug in tx callback of the CndSwCmd.
   * Before sending a CndSwCmd frame now the m_application_param_options 
     get initialised.

** Comments 
   * 
	 
	 
Version 0.2.9 - 20140731
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Restart of the blinking if the first long keypress is 
     longer than 10s during factory reset.
   * Removed pullUp from inputPin of the Reed-contact.
   * Now Parameters of List1 can be set correctly.

** Comments 
   * New version of HMOS (release 91049).
   * Before going to sleet the pullUp of the sabotage input 
     now gets disabled.
   
   
Version 0.2.8 - 20140730
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * After successfull sending now LED_PROGRAM_SUCCESS_SHORT is
     the correkt LED-programm.

** Comments 
   * Again modified the factoryReset mechanism.
   
   
Version 0.2.7 - 20140730
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed some warnings.
   * Fixed a bug in APPLICATION_STATE_VALIDATE_GET_PARAM1.

** Comments 
   * New version of HMOS (release 91004).
   * Some Changes with the LEDs due to new HMOS version.
   * On inclusion the including AC will be set as StatusInfo receiver.
   
   
Version 0.2.6 - 20140728 (THIS VERSION WAS SEND TO BOSCH AS FIRST 40 SAMPLES)
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected listen mode (in inclusion request).

** Comments 
   * 
   
   
Version 0.2.5 - 20140725
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New version of HMOS (release 90811).
   * Added CYCLIC_INFO_MSG from List0.
	 
	 
Version 0.2.4 - 20140724
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * ConfigUpdateRequests are now send to the access-controller 
     and not longer to the statusInfor receiver.

** Comments 
   * Readded sending of a ConfigUpdateRequest frame due to an 
     empty partner list. (commendet in 0.1.2)
	 
	 
Version 0.2.3 - 20140724
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed m_b_optic_present.
   * Removed dbg_toggle.
   * Fixed a bug that caused toggling of the inclusion mode 
     after factory reset.

** Comments 
   * Added m_b_status_changed to mark that the next cyclic 
     message has to pass filter_B.
   * Added BOOT flag to the StatusInfo telegramm. Due to this 
     change the mechanism of setting the bidi-bit was modified.
   * Added functionality to send a bidi StatusInfo regularly 
     (each 30th -> approx. each hour).
   
   
Version 0.2.2 - 20140723
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New version of HMOS (release 90748).
   * Added em_rmu.c and em_wdog.c to the project.
	 
	 
Version 0.2.1 - 20140722
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Now really removed EMV_MODE from config.h.
   * Now blinking orange on factory reset.

** Comments 
   * New version of HMOS (release 90655).
   * Changed device type to the official ones.
   * Changed initial values of m_b_StatusInfo_ACKed and 
     m_b_CndSwCmd_ACKed to __TRUE.
   * Added reset of m_b_StatusInfo_ACKed and m_b_CndSwCmd_ACKed
     on timeout.
   * Added PARTNER_SNC_ID (temporarly / for testing) to the 
     default listener of StatusInfo telegramms (in handling 
	 routine of ACKs). 
	 Maybe this has to be changed back later!
   
   
Version 0.2.0 - 20140722
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Removed EMV_MODE from config.h because it is not longer 
     necessary.
   * Corrected Paramter lists.
   * Corrected a bug in StatusInfo.

** Comments 
   * Moved some defines from frames.c to frames.h.
   * Added function prototypes to the top of allication.c.
   * Added default values to the parameter lists.
   * Added processing of ACKs.
   
   
Version 0.1.4 - 20140716
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * New version of HMOS.
   
   
Version 0.1.3 - 20140716
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added compiler-switch ENDLESS_FAST_INCLUSION to activate 
     endless inclusion in 1s intervall for EMV.
   * Created two new targets for EMV.
   
   
Version 0.1.2 - 20140715
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * A not included optical sensor doesn't send CndSwCmds anymore.
   * Corrected detection of the REED-contact.

** Comments 
   * Added sending of a not cyclic StatusInfo if the window 
     status changed. Also decreased the "priority" of the StatusInfo, 
	 so that first all CndSwCmd will be send.
   * Commented "m_application_pending.config_request = __TRUE;" 
     to avoid sending a configUpdateRequest after a send of a 
	 CndSwCmd has failed due to an empty partner buffer.
   * Added possibility to send the StatusInfo as a BiDi frame.
   
   
Version 0.1.1 - 20140714
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added functionality of parameter filter_a and filter_b.
   * Added functionality of parameter local_reset_disable.
	 
	 
Version 0.1.0 - 20140714
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected StatusInfo frame. Now sorted by type.
   * Removed KeyState from params of StatusInfo and CndSwCmd
     because it is not used in the shutter contact.

** Comments 
   * Added local variables for some parameters in list 0 and list 1.
   * Changed setting of the lowbat flag. Now the value out of 
     the parameters will be used not longer a fixed value.
   * Changed creating CndSwCmd frame. Now the parameter 
     MSG_POS_FOR of list1 is used to set the decision value.
   
   
Version 0.0.17 - 20140710
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added handling of list 1.
   
   
   Version 0.0.16 - 20140708
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Corrected used power mode.
   * Removed the keycheck of the factory reset from firstboot 
     to general state in the init routine of the application. 
	 Now a reset is possible on each boot.

** Comments 
   * New version of HMOS.
   
   
Version 0.0.15 - 20140707
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed size of APPLICATION_LIST0_CREATE_BUFFER to 8.
   * Corrected gesture of the factory reset and some depending 
     issues.

** Comments 
   * 
	 
	 
Version 0.0.14 - 20140703
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Added Measurement of the battery from external source for 
     the optic version of the shutter contact.
   * Sorted StatusInfo content by type.

** Comments 
   * Added status of the sabotage swich to the StatusInfo frame.
   * Added Error-Byte to the StatusInfo frame.
   * Added compile-switch  OPTIC_PRESENT to differ between the 
     optical and the magnet version of the contact sensor at 
	 compile time instead at runtime.
	 
	 
Version 0.0.13 - 20140701
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Fixed bug with StatuInfo Type.
   * Sorted StatusInfo content by Channel.

** Comments 
   * 
	 
	 
Version 0.0.12 - 20140630
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added DUMMY-factory-reset on key release after long press.
	 
	 
Version 0.0.11 - 20140630
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added toggeling of inclusion mode on config key when not 
     included (for debug).
		
		
Version 0.0.10 - 20140627
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added DUMMY_DEVICE_NUMBER to config.h.
   * Added ConfigRequest.
   -> ATTENTION: Due to no recipient the ConfigRequest can not 
		be tested now!
		
		
Version 0.0.9 - 20140626
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Changed BUFFER_append() to BUFFER_set_data() in 
	 APPLICATION_STATE_VALIDATE_SET_STATUSINFO_RECEIVER
	 due to codesize and speed.

** Comments 
   * Changed mode of the sabotage key to switch.
   * Added rx_sleep_delay to keep the device awake for 5 seconds 
     after sending any frame.
   * Added cyclic sending of the StatusInfo frame.
   -> ATTENTION: local counter instead of sequenceNumber used!
		-> Noone can synchrinise to it!
   
   
Version 0.0.8 - 20140625
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * Now Starting RX-mode after sending an inclusion request.
   * Readded HMIP_APP_receive_async-function to the project to 
     fix the inclusion.

** Comments 
   * Removed USE_HAL_AES_IN_APPLICATION_ONLY from hm-config.h.
   * Changed DEVICE_INFO_OPERATION_MODES to DEVICE_OPERATION_MODE_LISTEN_CYCLIC.
   * Added sending of StatusInfo telegramms.
	 
	 
Version 0.0.7 - 20140620
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Added Sleep-mode functionality (updated the stack and 
     changed the rx behaviour of the application).
   
   
Version 0.0.6 - 20140617
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed unnecessary initialisation of some buffers.
   * Added sending of CndSwCmd.
   
   
Version 0.0.5 - 20140606
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Removed some unused stuff from the example.
   * Added states to send CndSwCmd and StatusInfo to the application_do.
   * Added factory-function to build the CndSwCmd.
   
   
Version 0.0.4 - 20140603
--------------------------------------------------------------

** Related Hardware
   * 1343958F / 1454161A

** Bugfix
   * 

** Comments 
   * Ported Firmware to the new PCB of the Bosch TFK.
   * Added some reed-contact content.
	 
	 
Version 0.0.3 - 20131125
--------------------------------------------------------------

** Related Hardware
   * 1343958F

** Bugfix
   * 

** Comments 
   * Added IR-Sensor functionality and connected it to 
     LED (for debug purposes). Sending of CndSwCmd to all 
	 partner missing.
	 
	 
Version 0.0.2 - 20131125
--------------------------------------------------------------

** Related Hardware
   * 1343958F

** Bugfix
   * 

** Comments 
   * Implemented newstart of the inclusion process after the 
     keyvisual was pressed.
   * Improved Versioning of the project.
	 
	 
Version 0.0.1 - earlier
--------------------------------------------------------------

** Related Hardware
   * 1343958F

** Bugfix
   * 

** Comments 
   * Initial commit with template as new start of the project.
	 
	 
--- END OF FILE ---



Version <Versionsnummer> - <Releasedatum im Format YYYYMMDD>
--------------------------------------------------------------

** Bugfix
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des allgemeinen Fehlers bzw. Programmabsturzes>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des allgemeinen Fehlers bzw. Programmabsturzes>

** New Feature
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der neuen Funktion>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der neuen Funktion>

** Modification
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Modifikation>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Modifikation>

** Improvement
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Verbesserung>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Verbesserung>

** Bugs
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des offenen Fehlers>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des offenen Fehlers>

** Related Hardware
   * <Platinennummer> - <zusätzliche Hinweise, Modifikationen usw.>

** Comments
   * <Allgemeiner Kommentar>
   * <Allgemeiner Kommentar>

