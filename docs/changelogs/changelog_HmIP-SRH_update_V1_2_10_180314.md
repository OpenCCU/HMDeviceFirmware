## [HmIP-SRH_update_V1_2_10_180314.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-SRH_update_V1_2_10_180314.tgz)
Required CCU firmware version: &#8805; 3.37.8 / 2.33.3<br/>
<sub>sha256: 1746feadae1f219a915e0a216dca0d2755b89333d49147950aca5ffb84a0e364</sub>

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit der aktuellsten CCU2/3 Version.

Please note: Only use the firmware file in connection with the latest CCU2/3 version.

Changelog: 

Version 1.2.10 - 20180312
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * [HMIP_SRH-21]Fixed a bug that caused setting of alarmworthy 
     event flag with unidirectional or cyclic status frames.

** Comments 
   * 
   
   
Version 1.2.8 - 20180308
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Fixed a bug with receiving answers of conditional switch commands.

** Comments 
   * 
   
   
Version 1.2.6 - 20180219
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * 

** Comments 
   * Changed counting of event_counter to new mechanism
     (boot:0; other:[1..252]). [CHANGEMANAGEMENT-483]
	 [HMIP_SRH-20]
   * Reworked the mechanism of receiving answers.
   
   
Version 1.2.4 - 20180209
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Added separate keypress counter for window and backup.
   * All pending flags are now handled after boot process is 
     finished. Otherwise it is possible to miss an acknowledgment  
     frame of a frame at boot.

** Comments 
   * 
   
   
Version 1.2.2 - 20180207
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Added first statusinfo to the backup mechanism.

** Comments 
   * 
   
   
Version 1.2.0 - 20180205
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * 

** Comments 
   * HMOS 1.20.4
   * Increased version due to creation of a tag.
   
   
Version 1.1.5 - 20180201
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Added mechanism to prevent overwriting of a alarmworthy 
     event with a not alarmworthy one.
	 -> Fast window open and close now also causes a backup.

** Comments 
   * 
	 
	 
Version 1.1.4 - 20180201
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Fixed a bug with missing MAC_ACKs after blinking.
     [HMIP_SRH-18]

** Comments 
   * Added new parameter DISABLE_MSG_TO_AC.
     [HMIP_SRH-17][CHANGEMANAGEMENT-223]
	 
	 
Version 1.1.3 - 20180201
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * 

** Comments 
   * Added alarm-channel and depending functionality for 
     security solution
   
   
Version 1.1.2 - 20170803
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Fixed bug in sleep behaviour.
     [HMIP_SRH-11][CHANGEMANAGEMENT-100]

** Comments 
   * 
   
   
Version 1.1.1 - 20160425
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Fixed a bug with ACKs to config update request frames.

** Comments 
   * 
   
   
Version 1.1.0 - 20160413
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * 

** Comments 
   * Incremented version number due to creation of a tag.
   
   
Version 0.3.0 - 20160408
--------------------------------------------------------------

** Related Hardware
   * 1624316C

** Bugfix
   * Now the device sends statusinfo after boot (again).
   * Added receiving of status request frames.

** Comments 
   * Incremented version number due to creation of a tag.
   
   
Version 0.1.6 - 20160317
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * Corrected a bug with the first cyclic status info frame.

** Comments 
   * 
   
   
Version 0.1.5 - 20160316
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * Fixed a bug with switching LEDs in Testmode.

** Comments 
   * 
	 
	 
Version 0.1.4 - 20151001
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   *

** Comments 
   * Changed the reset precedure to the new rules.
     (no device functionality and boot blinking during reset, 
	 restart of the device if reset is not done correctly or 
	 gets aborted)
   * Parameter now get loaded on startup to be abble to do the 
     factory reset (local reset needs to be checked).
   * Changed Full RX timeout between sending start and the 
     callback from ARR-timout to a fix value (1000000) to be 
	 able to check the new router functionality.
	 
	 
Version 0.1.3 - 20150902
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * Again corrected default values for filterA and filterB.
     (made mistake in version 0.1.1)   
   * YOU_CTS_OPT_SMI_BN-29 - The Full RX mode of the trx is 
     retriggered in the tx callback of the conditional switch 
     command.

** Comments 
   * Set the input of the sensor keys to floating to avoid 
     unnecessry current consumption.
   * Removed activating of internal pullUp of the sabotage 
     input after sleep.
   * Added sending of link partner problem frames after 
     not receiving a MAC_ACK.
   
   
Version 0.1.2 - 20150805
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * Corrected testframe for the two sensor buttons.
   * Corrected device type.
   * Corrected a bug with the delay time made in the past version.
   * Removed workaround for missing pullups.

** Comments 
   * 
   
   
Version 0.1.1 - 20150730
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * Corrected the polarity of the LED.
   * Corrected pinout of the buttons.
   * Corrected default values for filterA and filterB.
   * Corrected default value for message position.
   * Corrected default value for event delay.

** Comments 
   * Removed Sample interval parameter.
	 
	 
Version 0.1.0 - 20150720
--------------------------------------------------------------

** Related Hardware
   * 1624316A

** Bugfix
   * 

** Comments 
   * Initial version. Due to the rotary handle sensor is similar 
     to the other contact sensors, this is a copy of the code.
	 
	 
--- END OF FILE ---



Version <Versionsnummer> - <Releasedatum im Format YYYYMMDD>
--------------------------------------------------------------

** Bugfix
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des allgemeinen Fehlers bzw. Programmabsturzes>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des allgemeinen Fehlers bzw. Programmabsturzes>

** New Feature
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der neuen Funktion>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der neuen Funktion>

** Modification
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Modifikation>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Modifikation>

** Improvement
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Verbesserung>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung der Verbesserung>

** Bugs
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des offenen Fehlers>
   * <JIRA Vorgangsnummer (optional)> - <Beschreibung des offenen Fehlers>

** Related Hardware
   * <Platinennummer> - <zusätzliche Hinweise, Modifikationen usw.>

** Comments
   * <Allgemeiner Kommentar>
   * <Allgemeiner Kommentar>

