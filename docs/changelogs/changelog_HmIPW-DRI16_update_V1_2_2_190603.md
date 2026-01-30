## [HmIPW-DRI16_update_V1_2_2_190603.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIPW/HmIPW-DRI16_update_V1_2_2_190603.tgz)
Required CCU firmware version: &#8805; 3.43.15<br/>
<sub>sha256: 0829a188be50d014eca08c1f20bf6842e94ce7ccff7c8ed7ca8ad9c68e9e1d0d</sub>

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIPW-DRI16 - Homematic IP Wired Input Module - 16 channels

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany

Version 1.2.2 - 2018-09-10
--------------------------------------------------------------

** Bugfix
   * If more than one status ACK frame is within the answer queue only the first
     one is send. Afterwards every new status ACK only triggers the last one
   * Statusinfo module creates status ACK telegrams with set ACK, ARR and Boot 
     bits if this is the first status to be sent after startup
   * HmIP_APP: Send node confusion when using external send nodes
   * Sometimes Statusinfo uses old ApplicationSequenceNumber and Statusinfo with ACK get lost


Version 1.2.0 - 2018-07-06
--------------------------------------------------------------

** Bugfix
   * If an input is configured as a switch, a long keystroke is sent when the input is opened.
   * Fix CCM flags according to RFC3610

** Improvement
   * Add new parameter for Contrast
   * Unify values for undervoltage


--- END OF FILE ---
