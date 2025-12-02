## [HmIP-SMI_update_V1_4_8_180228.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SMI_update_V1_4_8_180228.tgz)
<sub>sha256: 374c0999445e9ca15a9b74f645638922e04fded6a17b14a2718512e4ae06e7a8</sub>

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2(3) ab
Version 2(3).29.23

Please note: Only use the firmware file in connection with the CCU2(3) from
Version 2(3).29.23



Version 1.4.8 - 20180219
---------------------

** Bugfix
	* [HMIP_SMI-35]: A configuration of the PIR_OPERATION_MODE now influences the internal state for "motion_detection_on"
	* [HMIP_SMI-53]: Backup mechanism also triggered with NAK from SNC / StatusInfoReceiver. 

** Modification
	* [HMIP_SMI-51]: New handling of event_counter in CndSwCmds implemented.

** New feature
	* [HMIP_SMI-49]: Implementation of HmIP Security Solution PRO functionalities.




Version 1.4.6 - 20171208
---------------------

** Bugfix
	* [HMIP_SMI-47]: A multicast telegram on the state reset channel (ch 2) caused a rx_stop forever and an increased current consumption. 



Version 1.4.4 - 20171023
---------------------

** Bugfix
	*[HMIP_SMI-39]: Double ack after a received SwCmd generated an undefined frame that was sent out
	*[HMIP_SMI-41]: Non Ack_Status weren't sent with rssi code "unknown"
	*[HMIP_SMI-42]: Blink duty cycle signal once and send status if duty cycle limit is exceeded (status too when limit is undershot)




Version 1.4.2 - 20170927
---------------------

** Bugfix
	*[HMIP_SMI-35]: A configuration of the PIR_OPERATION_MODE now influences the internal state for "motion_detection_on"
	*[HMIP_SMI-36]: Only accept SwCmds from linkpartners on channel 2 for StateReset (not on channel 1) 
	*[HMIP_SMI-37]: Discard a ConfigReqUpdate when ACK of a LinkPartner wasn't received, but let pass them when triggered by a keypress
	*[HMIP_SMI-38]:	A status request causes a StatusAck which include a filtered and a current brightness. 
			Other StatusAck's (i.e. after DirExStop) causes a StatusAck which includes only a filtered brightness. 



** New feature
	*[HMIP_SMI-27]: Send two brightness values in a status_ack (1. Brightness = filtered, 2. Brightness = current)
	*[HMIP_SMI-28]: Reset motion state with blocking period when a switch command is received on the new channel 2 (input)
	*[HMIP_SMI-32]:	Added parameter for disabling messages to the access controller

** HMOS Version 
	1.16.0
	

Version 1.4.0 - 20170912
---------------------

** Bugfix
	*[HMIP_SMI-30]: Send a status acknowledge after switch on or switch off the motion detection by a direct execution start (with level = 0 or level != 0)

** Modification


** New feature
	*[HMIP_SMI-27]: Send two brightness values in a status_ack (1. Brightness = filtered, 2. Brightness = current)
	*[HMIP_SMI-28]: Reset motion state with blocking period when a switch command is received on the new channel 2 (input)
	*[HMIP_SMI-32]:	Added parameter for disabling messages to the access controller

** HMOS Version 
	1.16.0
	
** Comment
  

** Related Hardware
   * 1624300D - PCB for HmIP-SMI
   

Version 1.2.1 - 20160422
---------------------

** Bugfix
   send filtered brightness value in the response to request status info 

** Modification


** New feature
	
	

** HMOS Version 
	1.16.0
	
** Comment
  

** Related Hardware
   * 1624300D - PCB for HmIP-SMI
   

Version 1.2.0 - 20160411
---------------------

** Bugfix

** Modification


** New feature
	Dirict execution stop to cancel motion activ timer 

** HMOS Version 
	1.16.0
	
** Comment
  

** Related Hardware
   * 1624300D - PCB for HmIP-SMI
   
   
   
Version 1.0.4 - 20160310
---------------------

** Bugfix
   * the device was unable to handle the same IP address as Access Point and linkpartner 

** Modification


** New feature

** HMOS Version 
	1.14.1

** Related Hardware
   * 1624300D - PCB for HmIP-SMI

Version 1.0.3 - 20160120
---------------------

** HMOS Version 
	1.14.0

** Comment
  * initial version

** Related Hardware
   * 1624300D - PCB for HmIP-SMI
