## [hm_cc_rt_dn_update_V1_4_001_141020.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HM/hm_cc_rt_dn_update_V1_4_001_141020.tgz)
<sub>sha256: 4be8767661933366ae24d14c6a035d00dbe696115542a39c3c90a384e151567f</sub>

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

Version 1.4.001 - 14/10/20
--------------------------------------------------------------
** Bug
  * Modification the radio data interpretation function, if check for CONFIG_SERIALNUMBER it is also necessary to 
    check the frame typ for FRAME_CONFIGURATION.
  * Modification the direct link button-switch profile. 

Version 1.3.001 - 14/04/24
--------------------------------------------------------------
** Bug
  * Change in config_rt(...,...), parameter configuration is start at parameterposition 20.
    The weekly program transfer to the partner was incorrect if the first timestep > 21:15 o'clock
  * If party-mode bring into action, always the long status-message is send out instead of the 
    short status-message. The party-temperature is add as last byte at the long status-message.

Version 1.2.007 - 13/12/02
--------------------------------------------------------------
** Bug
  * If all shutter-contacts cleared from device and window-open-temperature is active, temperature return from 
    window-open-temperature to old temperature.
  * Internal window-open detection, send to partners.
  * Central-Order "Boost", "Comfort", "Lowering", "Change Temperature" still running, if Party-Pre-Stage is active.
  
** ChangeRequest  
  * The operation mode still shows in lcd if a thermal control is known.
  
Version 1.1.001 - 13/09/16
--------------------------------------------------------------
** Bug
  * Correction at takeover the actualtemperature and the settemperature, high-byte shift was not correct.
  * Correction at takeover ccu-radio-order, if internal window-open is detected, it has to reset.
  * Correction by the radio synchronization, if a thermal control is known, the device must synchronize to the
    radio-datapacket actual/set-temperature.