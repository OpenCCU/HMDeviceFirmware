## [HmIP-eTRV-2_I9F_update_V2_2_24_261001.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-eTRV-2_I9F_update_V2_2_24_261001.tgz)
Required CCU firmware version: &#8805; 3.65.11<br/>
<sub>sha256: c06821f1cd9d83a4b23edbc43bf262b4b93eaf1fc9820c1bbe25258f2e57f3a4</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIP-eTRV-2 - Homematic IP Radiator Thermostat

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 2.2.24 - 2026-10-01
--------------------------------------------------------------

** New Feature
   * The hydraulic balancing function was modified in consultation with TUEV Rheinland and the Berlin University of Applied Sciences. This modification was necessary to maintain the - HmIP-eTRVx Automatic Hydraulic Balancing of Space Heating Systems Using Electronic Control - certification.



Version 2.2.22 - 2024-05-03
--------------------------------------------------------------

** Bugfix
   * Communication problems with link partners if there is no cloud connection.
     If the cloud connection is lost, the Access point reports this to the device with
     a "Destination unreachable". This message causes a longer processing time in
     the device. During this time, the device cannot be reached by link partners.
     This can lead, for example, to window open/close messages not being received.



Version 2.2.20 - 2024-02-14
--------------------------------------------------------------

** Improvement
   * improve valve adaption noise immunity



Version 2.2.16 - 2022-10-06
--------------------------------------------------------------

** New Feature
   * First Release



--- END OF FILE ---
