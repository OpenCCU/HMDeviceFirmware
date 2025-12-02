## [HmIP-DRBLI4_update_V1_8_2_210216.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-DRBLI4_update_V1_8_2_210216.tgz)
<sub>sha256: 61d0159f4c9b52d0261aaab8038f1b709f54a8d8d9a708592e96edbaeb6a4be2</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIP-DRBLI4 - Homematic IP Jalousieaktor fÃ¼r Hutschienenmontage  â 4-fach

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 1.8.2 - 2021-02-15
--------------------------------------------------------------

** Bugfix
   * Section of virtual channels remains in "Move up/down reference run" if all three virtual channels are triggered by Direct Execution Command at startup



Version 1.8.0 - 2021-01-15
--------------------------------------------------------------

** Bugfix
   * A long keypress release leads to longer run time than the previous ones if the driving time is shorter than the long keypress repetition time
   * After a long button press, one channel will sporadically remain permanently supplied with 230 volts.
   * After a long keypress the actor runs longer than the set driving time
   * Device freezes, if undefined number of keypresses have been done



Version 1.6.0 - 2020-06-09
--------------------------------------------------------------

** Bugfix
   * Device sends RequestConfigUpdate if received a MacAck from a LinkPartner
   * The symbol for slat or shutter position remains in the display when switching to the input channels

** Improvement
   * Changing driving directions with HmIP UP actuators via parameters.
   * Add CHANNEL_OPERATION_MODE to switch between blind and shutter mode



Version 1.4.0 - 2019-09-24
--------------------------------------------------------------

** New Feature
   * Initial Release


--- END OF FILE ---
