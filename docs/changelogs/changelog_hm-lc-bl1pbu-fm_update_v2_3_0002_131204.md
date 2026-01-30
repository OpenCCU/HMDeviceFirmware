## [hm-lc-bl1pbu-fm_update_v2_3_0002_131204.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/hm-lc-bl1pbu-fm_update_v2_3_0002_131204.tgz)
<sub>sha256: c66a027195b022382c4c9acbee97b193914eaac2aa172b7030b23ce1f1c28868</sub>
Required CCU firmware version: &#8805; 3.0.0 / 2.9.0

In Verbindung mit der CCU2 wird das Gerät automatisch in den Updatemodus versetzt. 
Für ein Firmware-Update mit dem Firmware Update Tool, gehen Sie wie folgt vor:
1. Netzspannung ausschalten / vom Gerät trennen (Ggfs. Sicherheitshinweise der Installation beachten!),
2. den Aus/runter-Taster (UP-Markenschalter) bzw. den Bedientaster von Kanal 1 (sonstige Aktoren) drücken und festhalten,
3. bei immer noch gedrückt gehaltener Taste den Aktor wieder mit Netzspannung versorgen.
4. Sobald die LED schnell blinkt, kann die Taste losgelassen werden. Das Update wird jetzt durchgeführt.



Version 2.3.2 - 20131204
--------------------------------------------------------------
** Bugfix
   * Reset kann aus dem Anlernmodus heraus ausgeführt werden  
   * StatusInfo Verzögerung und Zufallsanteil falsch initialisiert
   * einschlafende Konfiguration bei AES aktiv
      
	  
Version 2.2.4 - 20130417
--------------------------------------------------------------
** Bugfix
   * Konfiguration über Offset + Liste war falsch umgesetzt
   * Sonderwert für Statusinfo inaktiv korrigiert (von 0xff auf 0)
   * Telegrammzähler bei Konfiguration korrigiert (zählte nicht hoch)  

** New Feature
   * Local-Reset-Disable eigebaut
   * Statusmitteilungen jetzt mit Random und Offset

** Improvement
   * Band belegt Prüfung bei Statusinfos eingebaut


Version 2.1.3 - 20120315
--------------------------------------------------------------
** Bugfix
   * Telegramm-Zähler bei Statusinfo zur CCU war immer Null
   * langer Tastendruck der internen Taste mit Profil up/down fehlerhaft
   
** New Feature
   * Bootloader kann per Funkbefehl aufgerufen werden
   * Versions-Nr. der FW per Info-Telegram übertragbar