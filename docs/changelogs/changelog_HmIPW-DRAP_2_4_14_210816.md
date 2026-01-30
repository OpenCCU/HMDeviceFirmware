## [HmIPW-DRAP_2_4_14_210816.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIPW/HmIPW-DRAP_2_4_14_210816.tgz)
<sub>sha256: 5f6ae794e45060b89e05649c8611f8be881e471bbcc393b2010b6fa21c0a18c8</sub>
Required CCU firmware version: &#8805; 3.61.5

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:      HmIPW-DRAP - Homematic IP Wired Access Point

Company:     eQ-3, Maiburger Str. 29, 26789 Leer, Germany



Version 2.4.14 - 2021-08-16
--------------------------------------------------------------

** Bugfix
   * Error Bus Ãberlastung im StatusInfo wird nicht zurÃ¼ckgesetzt
   * Carrier sense immer 0
   * The DRAP tries to start a sequence number validation on all frames and takes the destination address of the receiving frame as the source address.
   * HTTP client hangs if the previous connection was not closed.
   * The access point interrupts the connection to the cloud server if the lookup server has delivered an incorrect URL.
   * Sends to MulticastAllWiredDevices over Backbone with wrong CRRFD Address
   * Error with updateURL not accessible.
   * Websocket connection delay is only applied after restart.
   * DRAP (an einer CCU3) ist nach einem Firmware Update nicht mehr erreichbar
   * Full support for DEC Identify.
   * DRAP power supply rated current exceeded: DRAP display goes off, nothing else happens.
   * DRAP do not respond to IGMPv3 Membership Queries

** New Feature
   * Request Route to device for Live OTAU support

** Improvement
   * The web bootloader should prohibit a downgrade to a smaller major version.
   * If a DRAP is operated with 2 separate strings, multicast frames are sent to bus 1 and bus 2 one after the other - this could also happen simultaneously.



Version 2.2.24 - 2020-12-16
--------------------------------------------------------------

** Bugfix
   * Frames can no longer be sent. The stack remains in the busy state. 



Version 2.2.16 - 2020-09-23
--------------------------------------------------------------

** Bugfix
   * Download of update files will not start, if FIN,ACK from checkversion is not acked.



Version 2.2.12 - 2020-08-26
--------------------------------------------------------------

** Bugfix
   * Multicast Readressing is also applied to INTERFACE_LOCAL/CLOUD



Version 2.2.10 - 2020-08-24
--------------------------------------------------------------

** Bugfix
   * If the application is defective, an incorrect application version is reported to the update server.



Version 2.2.4 - 2020-08-07
--------------------------------------------------------------

** Bugfix
   * The device-specific configuration can no longer be retrieved with Netfinder.



Version 2.2.2 - 2020-07-24
--------------------------------------------------------------

** Bugfix
   * Wrong app sequence counter in status response frame.
   * In loop mode, inclusion request frames are discarded in the coprocessor.

** Improvement
   * Do not accept frames to AnyRouter if it is known that it is not routed.



Version 2.2.0 - 2020-07-16
--------------------------------------------------------------

** Bugfix
   * With the custom lookup address, the path is not processed correctly. 

** New Feature
   * Advanced Routing

** Improvement
   * change default update URL
   * Block duplicate multicast frames when routing.
   * Accept CCU SGTIN within Update Server URL
   * Changing from switching to routing between the two buses of the DRAP



Version 2.0.28 - 2020-02-24
--------------------------------------------------------------

** Bugfix
   * With the custom lookup address, the path is not processed correctly. 



Version 2.0.26 - 2020-10-13
--------------------------------------------------------------

** Bugfix
   * Download of update files will not start, if FIN,ACK from checkversion is not acked.



Version 2.0.22 - 2019-06-17
--------------------------------------------------------------

** Bugfix
   * No communication between RF and wired components 



Version 2.0.18 - 2019-04-08
--------------------------------------------------------------

** Bugfix
   * DRAP lights up orange after update.



Version 2.0.16 - 2019-02-05
--------------------------------------------------------------

** Bugfix
   * LED sequence for factory reset is to slow
   * Wrong DHCP Vendor ID. DRAP reports as HAP 

** New Feature
   * OTAU multicast frames have to be routed 



Version 2.0.12 - 2018-10-19
--------------------------------------------------------------

** Bugfix
   * If the DRAP is configured as a router and it sends a validation request before it gets an IP address from the DHCP server, the DRAP restarts. 
   * sometimes the watchdog is triggered while Bus is powering up 



Version 2.0.6 - 2018-08-27
--------------------------------------------------------------

** Improvement
   * Only evaluate the HTTP response code, not the response phrase. 



--- END OF FILE ---
