## [HmIP-eTRV-E-S_update_V1_6_12_261016.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-eTRV-E-S_update_V1_6_12_261016.tgz)
Required CCU firmware version: &#8805; 3.73.4<br/>
<sub>sha256: f57d86996502c4a224fa8266f5b3cc89e399232c084d411c2a53a56308a44668</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIP-eTRV-E - Homematic IP HeizkÃ¶rperthermostat â Evo

alte Bezeichnung:
Homematic IP HeizkÃ¶rperthermostat
HmIP-eTRV-E


Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version V1.6.12 - 2026-10-16
--------------------------------------------------------------

** Bugfix
   * The âWindow Openâ state triggered by a temperature drop detection on the eTRV link partner was not terminated.



Version V1.6.010 - 2026-09-28
--------------------------------------------------------------

** New Feature
   * The hydraulic balancing function was modified in consultation with TUEV Rheinland and the Berlin University of Applied Sciences. This modification was necessary to maintain the HmIP-eTRVx Automatic Hydraulic Balancing of Space Heating Systems Using Electronic Control certification.



Version V1.6.4 - 2025-06-24
--------------------------------------------------------------

** Bugfix
   * If the weekly profile is changed while in ECO mode, the set temperature will be set incorrectly. If you are in ECO mode and exit it, the previous temperature will be restored. However, if you are in ECO mode and switch to the weekly profile, the temperature set in the active profile will not be restored when you exit ECO mode.
   * Error code F2 is not displayed during operation
   * Window open symbol is not displayed when temperature drops
   * After a reinclusion, the device sometimes only reacts to a window contact after deleting and reintegrating. 
   * Device sends first Status without Bootflag when Sytempartner is set to Multicast Adress

** New Feature
   * Cooling function extension

** Improvement
   * Unnecessary valve movements were triggered when several window contacts were closed.
   * Improved error handling for configuration change notification on the device to the AP
   * The automatic switchover from manu-mode to auto-mode after a restart following receipt of the first time-info telegram should be deactivated.



Version V1.4.8 - 2024-09-23
--------------------------------------------------------------

** Bugfix
   * Changed define LOW_BAT_BOOT from 2.5V to 2.3V



Version V1.4.006 - 2023-10-17
--------------------------------------------------------------

** Bugfix
   * ARR Bit in CYCLIC_BIDI_INFO_MSG nicht gesetzt						
   * Low Bat Meldung kommt nicht bei Spannungseinbruch durch Motorfahrt / Display an
   * ARR Bit of Status Info Frame set False after Inclusion
   * Device sends ACK and NAK after Reboot command
   * Device reacts delayed after a window action with the motor drive



Version V1.4.004 - 2023-10-06
--------------------------------------------------------------

** Bugfix
   * ARR Bit of Status Info Frame set False after Inclusion

** Improvement
   * Status Info nach Ãnderung der Ventilposition wird spÃ¤t gesendet



Version V1.4.002 - 2023-09-19
--------------------------------------------------------------

** Bugfix
   * Valve-adapt: Device first sends Status "wait-state" before "adaption in progress"
   * Device sends ACK and NAK after Reboot command
   * Device sends Status Info to Multicast with ARR
   * Status info after window open has wrong valve level

** Improvement
   * Status Info nach Ãnderung der Ventilposition wird spÃ¤t gesendet



Version V1.4.000 - 2023-09-10
--------------------------------------------------------------

** Bugfix
   * When adaption is aborted via button press, the adaption is automatically restarted after installation drive
   * Device reacts delayed after a window action with the motor drive

** Improvement
   * Increase Low Batt Threshold



Version V1.2.002 - 2022-10-04
--------------------------------------------------------------

** Bugfix
   * Beleuchtungsdauer > 50 Sekunden stimmt nicht



Version V1.2.000 - 2022-02-10
--------------------------------------------------------------

** Bugfix
   * Setting vacation/party mode not possible
   * Valve remains closed after decalcification
   * eTRV kehrt nicht auf eingestellte Temperatur zurÃ¼ck nach Abschaltung des Eco-Modus



Version V1.0.012 - 2022-01-27
--------------------------------------------------------------

** Bugfix
   * Week program 3 not usable



Version V1.0.010 - 2021-03-01
--------------------------------------------------------------

** Improvement
   * Default value for display contrast must be adjusted



Version V1.0.000 - 2019-08-19
--------------------------------------------------------------

** Improvement
   * The time information telegram does not contain a note about the sommer / winter time change.



--- END OF FILE ---
