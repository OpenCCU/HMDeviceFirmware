## [HmIP-SPI_update_V1_2_4_171006.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SPI_update_V1_2_4_171006.tgz)
Required CCU firmware version: &#8805; 3.0.0 / 2.31.25<br/>
<sub>sha256: 813f884e0a6e4ed341c701a1353723ad5b5749d3e10b2e7b584e84261bcb14c7</sub>

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2 ab Version 2.31.25
Nach dem erfolgreichen Übertragen des Updates ist es erforderlich den HmIP-SPI einmal von der CCU2 ab- und wieder anzulernen, damit alle neuen Funktionen in der CCU2 korrekt angezeigt werden.

Please note: Only use the firmware file in connection with the CCU2 from version 2.31.25
After the update has been successfully transferred, it is necessary to disconnect the HmIP-SPI from the CCU2 and teach-in the device again. So that all new functions are displayed in the CCU2.

Changelog: HmIP-SPI

Version 1.2.4 - 20170922
---------------------

** Bugfix
   * [HMIP_SPI-37]:	Only accept SwCmds from linkpartners on channel 2 for StateReset (not on channel 1)
   * [HMIP_SPI-38]:	A status request causes a StatusAck which include a filtered and a current brightness. 
			Other StatusAck's (i.e. after DirExStop) causes a StatusAck which includes only a filtered brightness. 
   

Version 1.2.2 - 20170919
---------------------

** Bugfix
   * [HMIP_SPI-34]:	Switch commands on channel 1 now don't cause a presence state reset with a subsequent blocking period (this works only on channel 2)
   * [HMIP_SPI-35]:	Added parameter for disabling messages to the access controller
   * [HMIP_SPI-36]:	A configuration of the PIR_OPERATION_MODE now influences the internal state for "presence_detection_on"
   

Version 1.2.1 - 20170901
---------------------

** Bugfix
   * [HMIP_SPI-31]:	Send Status after config PIR_OP_MODE if value differs to the old one
   * [HMIP_SPI-32]:	Updated HMOS Version to V1.20.3 for fixing problem with communication with device before boot status was sent
   * [HMIP_SPI-33]:	Direct Execution Stop must only reset the current presence detection state and not the presence detection mode (On/Off) incremented already the patch
   
 

Version 1.2.0 - 20170815
---------------------

** Bugfix
   * [HMIP_SPI-9]:	Send Status if DutyCycle threshold (default at 90% DutyCycle) is crossed ( rising + falling )
   * [HMIP_SPI-26]:	Send Status_Ack after DirectExecCmd - Start or - Stop to switch detection_mode on/off
   * [HMIP_SPI-27]:	Send Status directly after inclusion + ensure synchronisation of acyclical status (no other status must not affect this)
   
** Modification
   *

** New feature
   * [HMIP_SPI-22]: Presence detection can be deactivated with a subsequently blocking period by receiving UnCndSwCmds or CndSwCmds on a new input channel (channel 2)
   * [HMIP_SPI-22]: Presence detection can be deactivated with a subsequently blocking period by receiving LevelCmds on a new input channel (channel 2)


Version 1.0.0 - 20170301
---------------------
	
** Comment
   *  Initial Release / First Version
