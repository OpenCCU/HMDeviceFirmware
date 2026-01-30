## [HmIPW-FALMOT-C12_update_V1_4_6_210209.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIPW/HmIPW-FALMOT-C12_update_V1_4_6_210209.tgz)
<sub>sha256: 8d77f95a614ac9dde8f5fc7cd26ae153b3dc3f0b84dac49af3e3bbf8da6f1545</sub>
Required CCU firmware version: &#8805; 3.57.5

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:   HmIPW-FALMOT-C12 - Homematic IP Floor Heating Actuator â 12 channels, motorised

Company:  Q-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1.4.006 - 2021-02-09
--------------------------------------------------------------
** Bugfix
   * FALMOT reports disconnection to WTH if "Window open" is reported by WTH for longer
     than 3 hours.
      As soon as window open was signaled by the WTH, the cyclic telegram set/actual
      temperature from the WTH was no longer processed by the device, i.e. set and
      actual temperature were not updated until window close.
   * When the time request changes to the WTH partner, it does not change back to the
     Access Point
      If the Access Point is not reachable, the time request is sent to a known WTH. The
      time request was then sent permanently to this partner. This led to increased data
      communication if routers in the field.


Version 1.4.002 - 2020-11-30
--------------------------------------------------------------

First Release.


--- END OF FILE ---

