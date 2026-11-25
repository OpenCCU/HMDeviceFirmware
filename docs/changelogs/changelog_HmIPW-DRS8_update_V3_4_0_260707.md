## [HmIPW-DRS8_update_V3_4_0_260707.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIPW/HmIPW-DRS8_update_V3_4_0_260707.tgz)
Required CCU firmware version: &#8805; 3.43.15<br/>
<sub>sha256: 214f7cd0ed34787aae1d1dbed4f2d56c52791959464f4a01f62144c5cb86d17a</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIPW-DRS8 - Homematic IP Wired Switch Actuator - 8 channels

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 3.4.0 - 2026-07-07
--------------------------------------------------------------

** Bugfix
   * Device only switches the relay back to the initial state when voltage is applied again after a power failure.
   * Undefined behavior after undervoltage switch-off
   * In a switching profile with all 8 channels, channel 8 sporadically does not switch
   * Wrong evaluation of the event counter with multiple links between sensor and actuator
   * If the switch-on and switch-off times in the Easy Profile are set to "Not active" at the same time, the device hangs up.
   * Event counter timeout isn't reset if within the triggered profile the multiexecution flag isn't set
   * Short key press of key visual leads to a restart, if a factory reset was aborted before
   * Weekprogram is sometimes not executed for all channels

** Improvement
   * The time information telegram does not contain a note about the sommer / winter time change.
   * Modify event counter check to meet current specification



Version 1.2.6 - 2022-09-28
--------------------------------------------------------------

** Improvement
   * new HMOS Version



Version 1.2.4 - 2018-08-27
--------------------------------------------------------------

** Bugfix
   * If more than one status ACK frame is within the answer queue only the first one is send. Afterwards every new status ACK only triggers the last one
   * Statusinfo module creates status ACK telegrams with set ACK, ARR and Boot bits if this is the first status to be sent after startup
   * HmIP_APP: Send node confusion when using external send nodes
   * Sometimes Statusinfo uses old ApplicationSequenceNumber and Statusinfo with ACK get lost
   * Answer-Frames are sometimes sent to the wrong IP destination
   * Weekprogram doesn't work correctly if several virtual channels shall be triggered by one switching point



Version 1.2.2 - 2018-07-05
--------------------------------------------------------------

** Bugfix
   * Profile: Buffer for learned links can overflow



Version 1.2.0 - 2018-07-03
--------------------------------------------------------------

** Bugfix
   * If the link partner is known, an NAK is sent on ("invalid") frames without ARR bit
   * If "Disable Message to AC" is activated and only one channel is addressed, no App-Ack is sent.
   * Direct Execution Commands without ARR bit are answered at application level
   * Homematic IP actuators trigger, due to the astro function, one hour delayed or prematurely on the day of the time changeover.
   * Divide maximum number of partners for virtual channels into individual values for virtual A, B and C
   * Fix CCM flags according to RFC3610
   * With "Overheat" the actuator can still be switched manually

** Improvement
   * All PowerUp parameters, that are listed in list 3 of the device, must be supported.
   * Add new parameter for Contrast
   * Unify values for undervoltage
   * Increase interval for switching actuator channels after power up



--- END OF FILE ---
