## [HmIP_STHD_update_2_2_2_170929.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP_STHD_update_2_2_2_170929.tgz)
<sub>sha256: c766f98ccb79865fdd28e747aab367701e1330b52281c4cce28a8974b0e1e6e0</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.29.22

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2 ab
Version 2.29.22

Please note: Only use the firmware file in connection with the CCU2 from
Version 2.29.22

Changelog: HmIP-WTH, HmIP-STH, HmIP-STHD


Version 2.2.002 - 20170929
----------------------------------------------------------------------------------------
Version:
  Application:  2.2.000
  Bootloader:   1.8.000
  Library:      1.20.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Missing port initialization for the HmIP-STHD
     The setpoint temperature can be changed by static charging.

** Modification
  * Change to Version 2.2.002


Version 2.2.000 - 20170918
----------------------------------------------------------------------------------------
Version:
  Application:  2.2.000
  Bootloader:   1.8.000
  Library:      1.20.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Correction in Paging-Module HMOS-Library
     Catched erros which could occure after an OTAU update to a newer paging module.
  * Correction for the Optimum Start Stop function
     After activating the optimum start stop function it is now executed correctly.

** Modification
  * Change to Version 2.2.000
     With the help of the new parameter "DISABLE_MSG_TO_AC" all transmissions to the
     central address are suppressed. Also to the status receiver address if this is the
     same as the central address.


Version 2.0.000 - 20170721
----------------------------------------------------------------------------------------
Version:
  Application:  2.0.002
  Bootloader:   1.8.000
  Library:      1.20.003

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Correction when trying changing from manu mode to auto mode if the time is not known.
     In manu mode boost is not activated by a long button press if the time is not known.

** Modification
  * Change to Version 2.0.002


Version 2.0.000 - 20170720
----------------------------------------------------------------------------------------
Version:
  Application:  2.0.000
  Bootloader:   1.8.000
  Library:      1.20.003

** Related Hardware
  * 1434158F, 1434177A

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
  * Correction when trying changing from manu mode to auto mode if the time is not known.
     In manu mode boost is not activated by a long button press if the time is not known.
  * Abort of Quick Veto by "Duration = 0".
     If Quick Veto is active, Quick Veto can be aborted by the radio command
     "Duration = 0". The device answers the radio telegram with an "Ack".

** Modification
  * Change to Version 2.0.000


Version 1.8.004 - 20170328
----------------------------------------------------------------------------------------
Version:
  Application:  1.8.004
  Bootloader:   1.8.000
  Library:      1.18.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Bug fixing optical system LED flashing
     The corresponding system LED flashing sequence has not been reproduced correctly,
     if the factory set was not be executable, because of the the LOCAL_RESET_DISABLE
     bit is set.
  * The hour was not taken into account during the transition from summer to winter time
    or from winter to summer time, so the conversion took place at 00:00.

** Modification
  * Change to Version 1.8.004


Version 1.8.003 - 20170215
----------------------------------------------------------------------------------------
Version:
  Application:  1.8.003
  Bootloader:   1.8.000
  Library:      1.18.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Bug fixing in temperature week program
     If one daily temperature profiles consist of only one switch time point, the switch
     time point is skipped by midnight of the next day.

** Modification
  * Change to Version 1.8.003


Version 1.8.002 - 20170227
----------------------------------------------------------------------------------------
Version:
  Application:  1.8.002
  Bootloader:   1.8.000
  Library:      1.18.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Improved handling at quick-veto
     Function is communicated to the link partner via a DEC-Command with "Duration-Time".

** Modification
  * Change to Version 1.8.002


Version 1.8.001 - 20170127
----------------------------------------------------------------------------------------
Version:
  Application:  1.8.001
  Bootloader:   1.8.000
  Library:      1.18.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * After bug fix no more cyclic messages were sent after a manual operation

** Modification
  * Change to Version 1.8.001


Version 1.8.000 - 20170124
----------------------------------------------------------------------------------------
Version:
  Application:  1.8.000
  Bootloader:   1.8.000
  Library:      1.18.004

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * New data packages will not be sent until the current data transmission has finished.

** Modification
  * Change to Version 1.8.000
  * Implementation of Quick-Veto-Function


Version 1.6.000 - 20160816
----------------------------------------------------------------------------------------
Version:
  Application:  1.6.000
  Bootloader:   1.8.000
  Library:      x.x.xxx

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * The Application_Sequence_Number for TIME_INFO_REQUEST is increment after sending.
  * If the device wait for incoming data, it don't responce to other requests.

** Modification
  * Change to Version 1.6.000


Version 1.5.001 - 20160608
----------------------------------------------------------------------------------------
Version:
  Application:  1.5.001
  Bootloader:   1.x.xxx
  Library:      1.x.xxx

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * If the device is linked with a Remote-Control-Unit and the Parameter "ON_TIME" is
    set, the temperature "TEMPERATURE_RC" is hold minimum for this time (also the time
    is > 1 Minute).
  * Expansion of the channel list, the device is linkable with a floor terminal 
    block (FAL).

** Modification
  * Change to Version 1.5.001
  * Some changes for testtunner for the new component HmIP-STHD
  * Some changes for testtunner for the new component HmIP-STH


Version 1.4.001 - 20160531
----------------------------------------------------------------------------------------
Version:
  Application:  1.4.001
  Bootloader:   1.8.000
  Library:      1.16.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Window open temperature isn't overwritten, when activating the party function.

** Modification
  * Change to Version 1.4.001


Version 1.2.013 - 20151209
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.013
  Bootloader:   1.8.000
  Library:      1.12.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.013


Version 1.2.012 - 20151209
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.012
  Bootloader:   1.8.000
  Library:      1.12.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Window open temperature isn't overwritten, when activating the party function.

** Modification
  * Change to Version 1.2.012


Version 1.2.011 - 20151111
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.011
  Bootloader:   1.8.000
  Library:      1.12.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.011


Version 1.2.010 - 20151111
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.010
  Bootloader:   1.8.000
  Library:      1.12.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * In combination with multiple routers the device is reached via radio all the time.
  * If a DEC is send with "actual temperature" and "4.5°C" as setpoint the device 
    performs nothing.

** Modification
  * Change to Version 1.2.010
  * Change in library -> m_rx_options.header.header.bidi to 
    m_rx_options.header.header.arr
  * Modification of full-rx-timeout in the application for router functionality.
  * Modification holiday period (start and end) must be transmitted as a status for
    CCU2 integration.


Version 1.2.009 - 20150824
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.009
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
   * 1434158F, 1434177A

** Modification
   * Change to Version 1.2.009


Version 1.2.008 - 20150824
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.008
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * All leap years are recognized.

** Modification
  * Change to Version 1.2.008


Version 1.2.007 - 20150702
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.007
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.007


Version 1.2.006 - 20150702
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.006
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * At window-open, a manually change on the device, is now transferred correctly from
    TRV link partners.

** Modification
  * Change to Version 1.2.006


Version 1.2.005 - 20150625
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.005
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.005


Version 1.2.004 - 20150625
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.004
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * Window status of SWD link partner is reset when the link partner is deleted.

** Modification
  * Change to Version 1.2.004


Version 1.2.003 - 20150624
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.003
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.003


Version 1.2.002 - 20150624
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.002
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * If the party mode is abort from the HAP, the party mode is immediately leave.

** Modification
  * Change to Version 1.2.002


Version 1.2.001 - 20150612
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.001
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.001


Version 1.2.000 - 20150612
----------------------------------------------------------------------------------------
Version:
  Application:  1.2.000
  Bootloader:   1.8.000
  Library:      1.10.000

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.2.000
  * Changeover the project to the hmos library


Version 1.0.017 - 20150624
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.017
  Bootloader:   1.8.000
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.0.017


Version 1.0.016 - 20150624
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.016
  Bootloader:   1.8.000
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * If the party mode is abort from the HAP, the party mode is immediately leave.

** Modification
  * Change to Version 1.0.016


Version 1.0.015 - 20150519
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.015
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Modification
  * Change to Version 1.0.015


Version 1.0.014 - 20150423
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.014
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * After inclusion the device send cyclic status messages.

** Modification
  * Change to Version 1.0.014


Version 1.0.012 - 20150422
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.012
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * After inclusion a Time-Date-Request is started.

** Modification
  * Change to Version 1.0.012


Version 1.0.010 - 20150421
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.010
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * The year 2100 and 2200 are not intercalary years.
  * Request of Date and Time only start if the TRX is not busy.

** Modification
  * Change to Version 1.0.010


Version 1.0.008 - 20150416
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.008
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * If "LowBat" and a Link-Partner doesn't send a answer for a DEC, the LED flash first
    600ms red and after that 200ms orange.

** Modification
  * Change to Version 1.0.008


Version 1.0.006 - 20150415
----------------------------------------------------------------------------------------
Version:
  Application:  1.0.006
  Bootloader:   1.4.001
  HMOS:         1.6.002

** Related Hardware
  1434158F, 1434177A

** Bugfix
  * If the parameter "ENABLE_ROUTING" is set, the device send not acknowledge package
    to anyrouter.
  * After change the parameter for the utc-offset, the device send a time request to
    the access point.

** Modification
  * Change to Version 1.0.006


Version 1.0.005 - 20150409
----------------------------------------------------------------------------------------

** Related Hardware
  * 1434158F, 1434177A

** Bugfix

** Modification
  * Change to Version 1.0.005


Version 1.0.004 - 20150409
----------------------------------------------------------------------------------------

** Related Hardware
  * 1434158F, 1434177A

** Bugfix
  * At DEC with temperature change the device furthermore pay attention for window open
    state.
  * Correction the evaluation of the filter parameters CYCLIC_INFO_MSG_DIS and 
    CYCLIC_INFO_MSG_DIS_UNCHANGED.
  * If a week program switch point is between 2:00 and 3:00 o'clock the device change
    setpoint temperature after change from winter to summer time.
  * Current consumption due to the status info message to the HAP with BiDi-Bit was too
    high.
  * After answer from HAP leave full rx mode.
  * Change values for status change check.
  * Boost Mode is also possible in Auto-Mode.
  * The setpoint temperature in Auto-Mode and in Party-Mode can only be in the range of
    5.0° <= setpoint <= 30.0°.
  * Parameter "ENABLE ROUTING" is evaluated.

** Modification
  * Change to Version 1.0.004


Version 1.0.003 - 20150320
----------------------------------------------------------------------------------------

** Related Hardware
  * 1434158F, 1434177A

** Bugfix

** Modification
  * Change to Version 1.0.003


Version 1.0.002 - 20150320
----------------------------------------------------------------------------------------

** Related Hardware
   * 1434158F, 1434177A

** Bugfix

** Modification
  * Change to Version 1.0.002


Version 1.0.001 - 20150319
----------------------------------------------------------------------------------------

** Related Hardware
  * 1434158F, 1434177A

** Bugfix

** Modification
  * Change to Version 1.0.001


Version 1.0.000 - 20150319
----------------------------------------------------------------------------------------

** Related Hardware
  * 1434158F, 1434177A

** Bugfix

** Modification
  * Change to Version 1.0.000