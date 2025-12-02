## [HmIP-FSI16_update_V1_18_22_2100623.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-FSI16_update_V1_18_22_2100623.tgz)
<sub>sha256: 77696c4ee8640228d6082a217a0bc77d3277edf94d55a9144c04955850c828be</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!
             If the switching actuator is operated in two-point control and the firmware version is 1.18.14, 
	     we recommend to remove the batteries from the wall thermostat until the actuator update has been 
             successfully done. Otherwise the transmission of the firmware will be interrupted.

Device:		HmIP-FSI16 - Switch Actuator (16 A) with Push-button Input - flush-mount

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
   * Device send status continuously after not receiving 
     application ack from central unit and 
     leads CCU and device running into duty cycle


Version 1 (2 for pluggable).18.12 - 20200622
--------------------------------------------------------------
** Bugfix
   * After inclusion, device sends bidirectional status telegrams
     to the CCU after approx. 120s


Version 1 (2 for pluggable).18.10 - 20200527
--------------------------------------------------------------
** Bugfix
   * BSM sends Statusframes with ARR every 3 minutes in case that 
     Central Unit does not send ack
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
   * Configuration is not longer shown on LED, if a key is pressed while getting config data

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

--- END OF FILE ---