## [hm-es-pmsw1-pl_update_v2_5_0009_150217.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/hm-es-pmsw1-pl_update_v2_5_0009_150217.tgz)
<sub>sha256: ea0b666edf8e6553cebb9167ab89d86d9592ea88f1b8e16d19cca365abcaea1a</sub>
Required CCU firmware version: &#8805; 3.0.0 / 2.9.0

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit dem Firmware Update Tool ab Version 1.1 sowie der CCU2 ab Version 2.9.10.
Die aktuellste Version des Firmware Update Tools finden Sie im Downloadbereich der Website www.eQ-3.de.

Please note: Only use the firmware file in connection with the Firmware Update Tool from version 1.1 as well as version 2.9.10 or higher of the CCU2.
You will find the latest version of the Firmware Update Tool in the download area of the website www.eQ-3.de.


In Verbindung mit der CCU2 wird das Gerät automatisch in den Updatemodus versetzt. 
Für ein Firmware-Update mit dem Firmware Update Tool, gehen Sie wie folgt vor:
1. Netzspannung des Gerätes ausschalten / vom Gerät trennen (Ggfs. Sicherheitshinweise der Installation beachten!),
2. den Bedientaster des Gerätes drücken und festhalten,
3. bei immer noch gedrückt gehaltener Taste den Aktor wieder mit Netzspannung versorgen.
4. Sobald die LED schnell blinkt, kann die Taste losgelassen werden. Das Update wird jetzt durchgeführt.


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