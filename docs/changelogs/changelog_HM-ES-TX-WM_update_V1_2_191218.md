## [HM-ES-TX-WM_update_V1_2_191218.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/HM-ES-TX-WM_update_V1_2_191218.tgz)
<sub>sha256: 63b655756e90e61e0d1841201c57cf8e8e410fcb5f893c299f48bf990d4826e6</sub>
Required CCU firmware version: &#8805; 3.45.7 / 2.45.7

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit dem Firmware Update Tool ab Version 1.1 sowie der CCU2 ab Version 2.15.2.
Die jeweils aktuellste Version finden Sie im Downloadbereich unter www.eQ-3.de.

Please note: Only use the firmware file in connection with the Firmware Update Tool from version 1.1 as well as from version 2.15.2 of the CCU2.
In each case you will find the latest version in the download area of www.eQ-3.de.

In Verbindung mit der CCU2 wird das Gerät automatisch in den Updatemodus versetzt.

Für ein Firmware-Update mit dem Firmware Update Tool, gehen Sie wie folgt vor:
1. Entnehmen Sie zunaechst die Batterien.
2. Den Anlerntasters (>) des Gerätes drücken und festhalten.
3. Mit gedrückt gehaltenem Anlerntaster die Batterien wieder einlegen.
4. Sobald die LED schnell blinkt, kann die Taste losgelassen werden. Das Update wird jetzt durchgeführt.

---------------------------------------------------------------------------------------------------------
| Wichtiger Hinweis bei dem Update von der Version 1.0:
|
| Dieses Update ist nur erforderlich, wenn Sie einen ES-IEC Sensor verwenden!
|
| Nach dem erfolgreichen Update ist ein Ablernen des Gerätes von der CCU, das Rücksetzen des Gerätes
| auf Werkseinstellungen und ein erneutes Anlernen an die CCU erforderlich.
---------------------------------------------------------------------------------------------------------

Changelog:

Version 1.2.001 - 20160628
--------------------------------------------------------------
** Improvement
  * ES-IEC
    * Reading Energy meter with protocol modes A and C
    * Passing negative power values on channel 1 to channel 2
  
Version 1.1.001 - 20160217
--------------------------------------------------------------
** Change Request
	* Sensor ES-IEC added
	
Version 1.0.002 - 20151218
--------------------------------------------------------------
** Release
	* Initial version