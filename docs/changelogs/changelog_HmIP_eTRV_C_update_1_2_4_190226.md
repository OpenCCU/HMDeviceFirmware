## [HmIP_eTRV_C_update_1_2_4_190226.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP_eTRV_C_update_1_2_4_190226.tgz)
<sub>sha256: bffdbac00406243673d50982869406115d0de9ccb58e3e94f37a042770379759</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device: HmIP-eTRV-C - Homematic IP Radiator Thermostat Compact

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1.2.004 - 2019-02-26
--------------------------------------------------------------

** Bugfix
   * Moving to the window open valve position happens twice.
      After opening the window, a new valve position is calculated. From time to time it
      happens that after moving to the new valve position, the valve move to the old
      valve position again for a short time.
   * Unconditional switch command to Multicast to wrong channel is answered.
      When receiving a unconditional switch command to the multicast address with wrong
      channel number, a nak was answered
   * Device does not respond to multicast AllTripleBurstListeningDevices.
      Frames with multicast address AllTrippleBurstListeningDevices was not responded.

** Modification
   * In "Duration" replace the unit "days" by "10ms".
      Revision of the current "Duration", since days are not needed as a unit for a
      16 bit value anyway.

** New Feature
   * Motor whisper mode
      The motor speed can be reduced by the parameter CHANNEL_OPERATION_MODE to minimize
      running noise.


Version 1.0.006 - earlier
--------------------------------------------------------------

First Release.

--- END OF FILE ---