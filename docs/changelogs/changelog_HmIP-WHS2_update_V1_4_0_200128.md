## [HmIP-WHS2_update_V1_4_0_200128.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-WHS2_update_V1_4_0_200128.tgz)
<sub>sha256: 06b5772974a28cc66a6487c2d91dc0a36aa1d5ae42c1c03eaa3a3b26e9057ff1</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device: HmIP-WHS2 - Homematic IP Switch Actuator for heating systems â 2 channels

Company: eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version HmIP-WHS2 V1.4.000
--------------------------------------------------------------

** Bugfix
   * Homematic IP actuators trigger, due to the astro function, one hour delayed or prematurely on the day of the time changeover.
   * Fehler in der Erzeugung des Wochenprogramm-Direct-Execution-Command

** New Feature
   * Firmware-Erweiterung erforderlich damit GerÃ¤t mit HmIP-FALMOT-C12 gepaired werden kann
   * AppSequenceCounter-Ãberwachung auf Bereich ausweiten

** Improvement
   * All PowerUp parameters, that are listed in list 3 of the device, must be supported



Version HmIP-WHS2 V1.2.000 - Not yet released
--------------------------------------------------------------

** Bugfix
   * Modus Anzeige vom WHS-2 wird nach Ãnderung nicht aktualisiert



Version  HmIP-WHS2 V1.0.004 - Not yet released
--------------------------------------------------------------

** Bugfix
   * Astrofunktion beim HmIP Wochenprogramm (fÃ¼r Aktoren) funktioniert nicht mit negativen LÃ¤ngen/Breitengraden

** New Feature
   * Definition von Zentralen basierten LÃ¶sungen und LÃ¶sungen ohne Zentrale (Installateur)



Version HmIP-WHS2 V1.0.002 - Not yet released
--------------------------------------------------------------

** Bugfix
   * Status Infos bei USC berÃ¼cksichtigen nicht das EVENT_DELAY
   * Falsche StatusInfo wenn alle KanÃ¤le Ã¼ber ein USC geschaltet werden
   * Zeitinformationen mit ARR-Bit werden nicht beantwortet

** Improvement
   * Parameter DAYLIGHT_SAVING_TIME im Default aktivieren



Version HmIP-WHS2 V1.0.001 - Not yet released
--------------------------------------------------------------

** Bugfix
   * Nach einem Request Status Info sendet das GerÃ¤t permanent die Status Info

--- END OF FILE ---
