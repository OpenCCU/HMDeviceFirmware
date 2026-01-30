## [hm-es-pmsw1-pl-dn-r1_update_v2_5_0009_150217.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/hm-es-pmsw1-pl-dn-r1_update_v2_5_0009_150217.tgz)
<sub>sha256: 3b397596abecc2ef1386fcf1642ecf530e1d679e7cd4363b475519899e654258</sub>
Required CCU firmware version: &#8805; 3.0.0 / 2.9.0

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der CCU2 ab Version 2.9.10.

Please note: Only use the firmware file in connection with the version 2.9.10 or higher of the CCU2.

Changelog:

Version 2.5 - 20141105
--------------------------------------------------------------
** Bugfix
   * before jump to bootloader, IRQs are disabled
   * problem with simulated telegrams fixed
   * toggle to counter was not correct
   * counter of internal buttonpress fixed
   * decode of transmitted time at conditional switch command fixed
   * ontime-mode minimum fixed

** Improvement
   * blinking enhanced to new definitions
   * ZC detection support
   * long buttonpress of device-button not only for config
   * power-up-action available
   * support for new devices
   * status messages with rising random interval 
   
   
Version 1.6 - 20140417
--------------------------------------------------------------
** Bugfix
   * fix delay for statusinfo when random time is set to zero

** Improvement
   * measured power sometimes not zero when relais is turned off


Version 1.5 - 20140204
--------------------------------------------------------------
** Modification
   * modification of TRX settings


Version 1.4 - 20131218
--------------------------------------------------------------
** Bugfix
   * energy counter goes wrong when power is above 300 W
   * device can be operated with its button, when device is locked by CCU