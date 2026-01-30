## [HmIP-PS-2_update_V2_22_0_211012.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-PS-2_update_V2_22_0_211012.tgz)
Required CCU firmware version: &#8805; 3.61.7 / 2.61.7<br/>
<sub>sha256: f5f384b3316a73573394d635cb452875a4bb537cdb331d699b47da7128bbc731</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:		HmIP-PS-2 - Homematic IP Pluggable Switch and Meter

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1 (2 for pluggable).22.0 - 20211008
--------------------------------------------------------------
** Bugfix
   * The time information telegram does not contain a note about the sommer / winter time change.
   * Timeout for first factory reset step is too long
   * Device sends RequestConfigUpdate if received a MacAck from a LinkPartner
   
** New Feature
   * Transmitting negative power from switching measuring actuators.
   * Overcurrent detection and shutoff (HmIP-PSM-2/HmIP-PS-2)
   
     
Version 1 (2 for pluggable).20.6 - 20211013
--------------------------------------------------------------
** Bugfix
   * Fixed Wrong definition of overload error flag
   * Fixed error if current is to big (e.g. 26 A -> if power is to big the power meter chip generates an power overflow, this caused a reset of power and current to 0)
   
** New Feature
   * Overcurrent detection and shutoff for switch actuators with metering (HmIP-PSM/HmIP-BSM/HmIP-FSM/HmIP-FSM16)


Version 1 (2 for pluggable).20.4 - 20210916
--------------------------------------------------------------
** Bugfix
   * The daylight saving time information is now taken from time information telegram, if included.
      
** Modification
   * Device sends RequestConfigUpdate if received a MacAck from a LinkPartner


Version 1 (2 for pluggable).20.2 - 20210825
--------------------------------------------------------------
** Bugfix
   * Update UART communication lib to fix a bug in power meter communication. 


Version 1 (2 for pluggable).20.0 - 20210722
--------------------------------------------------------------
** Bugfix

** New Feature
   * Support of HmIP-BSM-I
   * Reset of power meter chip if the communication is broken.


--- END OF FILE ---