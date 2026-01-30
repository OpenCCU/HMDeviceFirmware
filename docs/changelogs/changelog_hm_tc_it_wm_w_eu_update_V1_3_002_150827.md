## [hm_tc_it_wm_w_eu_update_V1_3_002_150827.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/hm_tc_it_wm_w_eu_update_V1_3_002_150827.tgz)
<sub>sha256: 0e88a6e4bf6a75f87851a26d14f4af2e31769bb42f7fe0e56d37cd14bd4d3eff</sub>
Required CCU firmware version: &#8805; 3.0.0 / 2.9.0

Achtung! Bitte verwenden Sie die Firmware-Datei nur in Verbindung mit dem Firmware Update Tool ab Version 1.1 sowie der CCU2 ab Version 2.9.0.

Die aktuellste Version des Firmware Update Tools finden Sie im Downloadbereich der Website www.eQ-3.de.

Please note: Only use the firmware file in connection with the Firmware Update Tool from version 1.1 as well as version 2.9.0 or higher of the CCU2.

You will find the latest version of the Firmware Update Tool in the download area of the website www.eQ-3.de.

In Verbindung mit der CCU2 wird das Gerät automatisch in den Updatemodus versetzt.

Für ein Firmware-Update mit dem Firmware Update Tool, gehen Sie wie folgt vor:

1. Entnehmen Sie bitte zunaechst die Batterien,

2. anschliessend sind die Batterien bei gleichzeitigem Druecken der Taster "Auto/Manu" und "Comfort/Eco" wieder einzulegen.

3. Im Display sollte nun "FUP" stehen. Das Update wird jetzt durchgeführt.


Changelog:

Version 1.3.002 - 15/08/27
--------------------------------------------------------------
** Bug
  * Fixed incorrect display at mode-lock.

  
Version 1.3.001 - 15/05/06
--------------------------------------------------------------
** Bug
  * Bugfix at direkt pairing. Sometimes the parameter configuration after pairing goes wrong.
** Change Request
  * The conditional data message for the two-point-regulation is send now cyclical.
  * If the button lock is active, the behaves of the lock symbol is simular to the HM-CC-RT-DN.

  
Version 1.2.001 - 14/10/20
--------------------------------------------------------------
** Bug
  * Modification the radio data interpretation function, if check for CONFIG_SERIALNUMBER it is also necessary to 
    check the frame typ for FRAME_CONFIGURATION.
  * Modification the direct link button-switch profile. 


Version 1.1.000 - 14/04/24
--------------------------------------------------------------

** Bug
  * Change in config_rt(...,...), parameter configuration is start at parameterposition 20.
    The weekly program transfer to the partner was incorrect if the first timestep > 21:15 o'clock
  * If party-mode bring into action, always the long status-message is send out instead of the 
    short status-message. The party-temperature is add as last byte at the long status-message.
** Change Request
  * Make direct pairing with HM-ES-PM-Sw1-Pl (Actor-Switch) possible.
  

Version 1.0.007 - 13/11/26
--------------------------------------------------------------

** Bug
  * If boost is activ, actual temp. and humidity are not show to display.
