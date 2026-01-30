## [HmIP-ESI_update_V1_4_0_240308.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-ESI_update_V1_4_0_240308.tgz)
Required CCU firmware version: &#8805; 3.73.9<br/>
<sub>sha256: 5064f670c40a14fa8ce9d1c1acc303c3741d8349c14669b2dece5389a1dcfad3</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIP-ESI - Homematic IP Energy Sensor Interface

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 1.4.0 - 2024-03-08
--------------------------------------------------------------

** Bugfix
   * Incorrect error message if IEC protocol not recognized
   * SML status word of length 1 byte not taken into account
   * no protocol detection of D0-D energy counter with 8-N-1 (LOGAREX)

** Improvement
   * Statusword under Obis 96.05.05 is not supported
   * fix DZG sign workaround
   * Error flashing if device is started without sensor
   * add OBIS 36.7.0 for single phase power meter
   * add workaround for Pafal EA5: take 'F' as 15 into OBIS C
   * Improved error handling for configuration change notification on the device to the AP
   * An ES-IEC without a recognized protocol should be reported



Version 1.2.2 - 2023-12-14
--------------------------------------------------------------

** Bugfix
   * Power consumption too high with ES-LED and ES-Gas
   * error code 1 on cloud inclusion

** Improvement
   * increase D0-C handshake timeout for LuG



Version 1.0.6 - 2023-11-02
--------------------------------------------------------------

** New Feature
   * First Release



--- END OF FILE ---
