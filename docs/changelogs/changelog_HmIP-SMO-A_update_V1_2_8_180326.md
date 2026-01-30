## [HmIP-SMO-A_update_V1_2_8_180326.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SMO-A_update_V1_2_8_180326.tgz)
Required CCU firmware version: &#8805; 3.37.8 / 2.33.3<br/>
<sub>sha256: 77e773ac02615346f1d43c991d9ace80a67e43cb0f1798a7d7a731f89a6ddd0f</sub>

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2(3) ab
Version 2(3).29.23

Please note: Only use the firmware file in connection with the CCU2(3) from
Version 2(3).29.23



Version 1.2.8 - 20180314
---------------------

** Bugfix
	*[HMIP_SMO-19]:	A configuration of the PIR_OPERATION_MODE now influences the internal state for "motion_detection_on"
	*[HMIP_SMO-32]: Backup mechanism also triggered with NAK from SNC / StatusInfoReceiver.
	*[HMIP_SMO-33]: Backup mechanism also triggered when MAC_ACK failed. 	

** Modification
	* [HMIP_SMO-30]: New handling of event_counter in CndSwCmds implemented.

** New feature
	* [HMIP_SMO-48]: Implementation of HmIP Security Solution PRO functionalities.

** HMOS Version 
	*

** Comment
  * [HMIP_SMO-19]: Lost state for validation of ch1 + ch2 parameter. Wrong flag was written in configuration.


Version 1.2.6 - 20171211
---------------------

** Bugfix
	*[HMIP_SMO-26]:	A multicast telegram on the state reset channel (ch 2) caused a rx_stop forever and an increased current consumption. 



Version 1.2.4 - 20171023
---------------------

** Bugfix
	*[HMIP_SMO-24]: Double ack after a received SwCmd generated an undefined frame that was sent out
	*[HMIP_SMO-25]: Non Ack_Status weren't sent with rssi code "unknown"


Version 1.2.2 - 20170927
---------------------

** Bugfix
	*[HMIP_SMO-19]: A configuration of the PIR_OPERATION_MODE now influences the internal state for "motion_detection_on"
	*[HMIP_SMO-20]: Only accept SwCmds from linkpartners on channel 2 for StateReset (not on channel 1)  
	*[HMIP_SMO-21]: Discard a ConfigReqUpdate when ACK of a LinkPartner wasn't received, but let pass them when triggered by a keypress
	*[HMIP_SMO-22]: A status request causes a StatusAck which include a filtered and a current brightness. 
			Other StatusAck's (i.e. after DirExStop) causes a StatusAck which includes only a filtered brightness. 




Version 1.2.0 - 20170913
---------------------

** Bugfix
	*[HMIP_SMO-16]: Send a status acknowledge after switch on or switch off the motion detection by a direct execution start (with level = 0 or level != 0)
	*[HMIP_SMO-12]:	Motion state reset didn't work correctly when parameter "CaptureWithinInterval" was set. Bug fixed in timer routine.

** Modification


** New feature
	*[HMIP_SMO-11]: Send two brightness values in a status_ack (1. Brightness = filtered, 2. Brightness = current)
	*[HMIP_SMO-13]: Reset motion state with blocking period when a switch command is received on the new channel 2 (input)
	*[HMIP_SMO-18]: Added parameter for disabling messages to the access controller

** HMOS Version 
	*

** Comment
  * 

** Related Hardware
   * 1634333F - PCB for HmIP-SMO
   
Version 1.0.0 - JJJJMMDD
---------------------

** Bugfix


** Modification


** New feature


** HMOS Version 


** Comment
  * initial version

** Related Hardware
   * 1634333C - PCB for HmIP-SMO
