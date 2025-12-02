## [HmIP_STHD_update_2_6_0_200131.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP_STHD_update_2_6_0_200131.tgz)
<sub>sha256: 6f737161afd35a2f44daf7e62c6bdb3a1b08233853db8896263620b7fb884a0a</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version
of the CCUx!

Device: HmIP-STHD - Homematic IP Temperature and Humidity Sensor with display - indoor

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 2.6.000 - 2019-09-04
--------------------------------------------------------------

** New Feature
   * Improvement for data communication.
      If possible the device send multicasts only to PARTNER_ALL_WIRED_DEVICES instead
      of to PARTNER_ALL_DEVICES.

** Improvement
   * Immediate evaluation of temperature change for the two-point-control.
      Temperature changes triggered by the central unit or a window contact, are
      forwarded directly to the switching actuators for the two-point-control.


Version 2.4.008 - 2019-03-07
--------------------------------------------------------------

** Bugfix
   * Logic "Window open temperature" corrected in cooling mode
      In cooling mode, it is not advisable to change to the window open temperature, as
      a result, more cooling would have to be used.
   * Error when changing from winter to summer time.
      On the day of the time change, the time is increased by one hour every full hour
      after 2 o'clock.

** Modification
    In "Duration" replace the unit "Days" by "10ms".
     Revision of the current duration, becaues a 16 bit value are not needed as unit
     "Days" anyway.

** Improvement
    Adjustment of the LCD start display
     In the future only the application version major minor will be shown in the LCD
     start display. All further information can be found in the app or the ccu.


Version 2.2.002 - 2017-09-29
--------------------------------------------------------------

** Bugfix
   * Correction when trying changing from manu to auto mode if the time is not known.
      In manu mode boost is not activated by a long button press if the time is not
      known.
   * Correction in Paging-Module HMOS-Library
      Catched erros which could occure after an OTAU update to a newer paging module.
   * Correction for the Optimum Start Stop function
      After activating the optimum start stop function it is now executed correctly.
   * Missing port initialization for the HmIP-STHD
      The setpoint temperature can be changed by static charging.

** New Feature
   * Parameter extension for installer solution.
      With the help of the new parameter "DISABLE_MSG_TO_AC" all transmissions to the
      central address are suppressed. Also to the status receiver address if this is the
      same as the central address.


Version 2.0.000 - 2017-07-20
--------------------------------------------------------------

** Bugfix
   * Correction for set point temperature update after weekprogram configuration.
      If window open is detected (extern/intern) and during this time a new week program
      is transmitted to the device, the device updated the set point temperature after
      window close by using the new week program set point temperature.
   * Extension for the Quick Veto Function.
      If the quick veto function is active, the remaining time is transferred in the
      status telegram.
   * Behavior after aborting the factory reset.
      If the factory reset is aborted or not executed until the end, the device performs
      a reboot after the termination or after the timeout.
   * Correction when trying changing from manu mode to auto mode if the time is not
     known.
      In manu mode boost is not activated by a long button press if the time is not
      known.
   * Abort of Quick Veto by "Duration = 0".
      If Quick Veto is active, Quick Veto can be aborted by the radio command
      "Duration = 0". The device answers the radio telegram with an "Ack".


Version 1.8.004 - 2017-03-28
--------------------------------------------------------------

** Bugfix
   * New data packages will not be sent until the current data transmission has
     finished.
   * After bug fix no more cyclic messages were sent after a manual operation
   * Improved handling at quick-veto
      Function is communicated to the link partner via a DEC-Command with
      "Duration-Time".
   * Bug fixing in temperature week program
      If one daily temperature profiles consist of only one switch time point, the
      switch time point is skipped by midnight of the next day.
   * Bug fixing optical system LED flashing
      The corresponding system LED flashing sequence has not been reproduced correctly,
      if the factory set was not be executable, because of the the LOCAL_RESET_DISABLE
      bit is set.
   * The hour was not taken into account during the transition from summer to winter
     time or from winter to summer time, so the conversion took place at 00:00.

** New Feature
   * Implementation of Quick-Veto-Function


Version 1.6.000 - 2016-08-16
--------------------------------------------------------------

** First release


--- END OF FILE ---