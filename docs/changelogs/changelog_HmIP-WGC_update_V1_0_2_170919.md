## [HmIP-WGC_update_V1_0_2_170919.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-WGC_update_V1_0_2_170919.tgz)
<sub>sha256: e3cb5b920e5c970329ab85621ade866f5e66416866a3a619765a5d4722f30970</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version
of the CCUx!

Device: HmIP-WGC - Homematic IP Wallmount Garage Controller

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 1.0.2 - 2017-9-1
--------------------------------------------------------------

** Related Hardware
   * 150948B

** Bugfix
 
** Improvement
   System turn off on voltage 2.0V
   Send the status frame with error bit to receiver once battery voltage under 2.4V
   Send the status frame with bad battery bit to receiver once battery voltage under 2.6V
   Once power by battery and the battery voltage is under 2.4V, no action on relay and send out an NAK frame.
   
Version 1.0.1
--------------------------------------------------------------

** Related Hardware
   * 150948B
   
** Comments
   * Updated to HMOS V1.20.3

Version 1.0.0 - 2017-8-14
--------------------------------------------------------------

** Related Hardware
   * 150948B

Release the version to V1.0.0


--- END OF FILE ---