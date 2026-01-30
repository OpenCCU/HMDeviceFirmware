## [HmIP_BWTH_update_1_2_4_180201.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP_BWTH_update_1_2_4_180201.tgz)
<sub>sha256: 6b67646c1c78610a7aad7c1404fa24d50423bbaf6e9346724cde9e27c0554863</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.31.25

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2 ab
Version 2.29.23

Please note: Only use the firmware file in connection with the CCU2 from
Version 2.29.23

Changelog: HmIP-BWTH, HmIP-BWTH24


Version 1.2.004 - 20171123
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.004
  Bootloader:   1.10.000
  Library:      1.20.004

** Related Hardware
   * HmIP-BWTH:   1664468x, 1454133x, 1333915x, 1333941x, 1333926x
   * HmIP-BWTH24: 1664468x, 1454133x, 1714486x, 1333941x, 1714485x

** Bugfix
  * Logic "Window open temperature" corrected in cooling mode
     In cooling mode, it is not advisable to change to the window open temperature, as
     a result, more cooling would have to be used.
  * Correction in Paging-Module HMOS-Library
     Catched erros which could occure after an OTAU update to a newer paging module.
  * Correction for the Optimum Start Stop function
     After activating the optimum start stop function it is now executed correctly.
  * Antenna symbol synchronization in the display.
    If the date and time can be requested by the access point, this is a sign that the
    radio communication is in order. The flashing of the antenna symbol should then be
    canceled.
  * Expansion for inclusion condition.
     If parameter changes have been made to the device before the inclusion, the device
     can only be included if a factory reset has been performed on the device before.
  * Correction for set point temperature update after weekprogram configuration.
     If window open is detected (extern/intern) and during this time a new week program
     is transmitted to the device, the device updated the set point temperature after
     window close by using the new week program set point temperature.
  * Function modification during two-point control.
     During the two-point control (startup sequence), the device do observe the
     parameter values "COOLING_DISABLE" and "HEATING_DISABLE".
  * Correction when changing from auto mode to manu mode.
     When changing from auto mode to manu mode and boost is active, boost is abort.
  * Function modification after removing internal link between channel 8 and channel 10.
     When removing the internal link between channel 8 and channel 10 by the access
     point, the relay should be deactivated.
  * Improvement for the display.
     When changing the temperature offset from the App the LCD display should be updated
     directly.
  * Extension for the Quick Veto Function.
     If the quick veto function is active, the remaining time is transferred in the
     status telegram.
  * Behavior after aborting the factory reset.
     If the factory reset is aborted or not executed until the end, the device performs
     a reboot after the termination or after the timeout.
  * Abort of Quick Veto by "Duration = 0".
     If Quick Veto is active, Quick Veto can be aborted by the radio command
     "Duration = 0". The device answers the radio telegram with an "Ack".

** Modification
  * Change to Version 1.2.004
     With the help of the new parameter "DISABLE_MSG_TO_AC" all transmissions to the
     central address are suppressed. Also to the status receiver address if this is the
     same as the central address.
  * Function modification of Optimum-Start-Stop
     Change to Optimum Start, means that the comfort temperature should be reached at
     the desired point in time, the lowering temperature not.


Version 1.0.011 - earlier
----------------------------------------------------------------------------------------

** Related Hardware
  * HmIP-BWTH:   1664468x, 1454133x, 1333915x, 1333941x, 1333926x
  * HmIP-BWTH24: 1664468x, 1454133x, 1714486x, 1333941x, 1714485x
