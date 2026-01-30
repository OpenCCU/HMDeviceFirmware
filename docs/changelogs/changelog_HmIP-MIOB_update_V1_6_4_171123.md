## [HmIP-MIOB_update_V1_6_4_171123.tgz](https://raw.githubusercontent.com/OpenCCU/HMDeviceFirmware/master/HmIP/HmIP-MIOB_update_V1_6_4_171123.tgz)
<sub>sha256: 8d3dcea6d6cb918df7e4774ed9e1245e3512a61482d2c428bfb42c3159fa133d</sub>
Required CCU firmware version: &#8805; 3.37.8 / 2.25.12

C H A N G E L O G
-----------------

Please note: Only use the firmware file in connection with the current software-version of the CCUx!

Device:		Multi Input/Output-Box for floor heating systems.

Company:	eQ-3, Maiburger Str. 29, 26789 Leer, Germany


Version 1.6.004 - 2017-11-23
--------------------------------------------------------------

** Improvement
	* MIOB behaviour in case of system restart improved. Now sends DEC-Logic to FAL in any case.
   
** Modification
	* Change to Version 1.6.004.

	
Version 1.6.002 - 2017-02-09
--------------------------------------------------------------

** Bugfix
	* In case of multiple FAL, linked to different acutator channels of the MIOB, in some configurations not all FALs got DEC Logic command (eg. for changeover).
   
** Modification
	* Change to Version 1.6.002.

	
Version 1.6.001 - 2017-02-08
--------------------------------------------------------------

** Bugfix
	* Fixed Issue: Direct execution command was sent to FAL on wrong Channel. If no Link between Out0 and FAL created, no DEC was sent from MIOB 
   
** Modification
	* Change to Version 1.6.001.

	
Version 1.6.000 - 2017-01-30
--------------------------------------------------------------

** Bugfix
	* Error in heat demand function (VIRT B-Channels of both actuators) fixed. 
   
** Modification
	* Change to Version 1.6.000.

	
Version 1.4.000 - 2016-09-20
--------------------------------------------------------------

** Bugfix
	* Issue with global pump protection function (in conjunction with the FAL) fixed.
   
** Modification
	* Change to Version 1.4.000.

Version 1.2.000 - 2016-09-08
--------------------------------------------------------------

** Bugfix

	* Fixed issue with powerup ontime and powerup ondelay at actuator channels.
	* Fixed issue with event delaytime and event randomtime for statusinfo 
	  transmission in case of statuschange at actuator channels.
	* Fixed issue with log keypress timer at application startup.
   
** Modification
	* Change to Version 1.2.000.

	
Version 1.0.012 - 2016-08-25
--------------------------------------------------------------

** Bugfix

	* Bugfix at internal link between input and output channels (CO-Pilot).
   
** Modification
	* Change to Version 1.0.012.

	
Version 1.0.011 - 2016-07-28
--------------------------------------------------------------

** Bugfix
	* Double ack at csc and usc fixed.
	* Application sequence counter error fixed.
   
** Modification
	* Change to Version 1.0.011.
	* Changed Lib to 1.16.1

	
Version 1.0.010 - 2016-07-28
--------------------------------------------------------------

** Bugfix
	* Bug with DEC of second relay output fixed
   
** Modification
	* Change to Version 1.0.010.
	* Unconditional switch command added for switching actuator channels
	

Version 1.0.009 - 2016-07-27
--------------------------------------------------------------

** Bugfix

	* Application ACK is now sent in case of set ARR Bit.  
	* Logic Combination fixed.
	* Powerupactions fixed.
	* Edit Parameterlist fixed.
   
** Modification
	* Change to Version 1.0.009.
	* Send Statusinfo subsequent to levelcommand or dec with level on channel for analog output.
	* Statusinfo is only sent in case of "significant" changes.
	

Version 1.0.008 - 2016-06-21
--------------------------------------------------------------

** Modification
	* Change to Version 1.0.008.
	* Minor changes in pairing routines.
	* Device Functions IDs adapted.

Version 1.0.007 - 2016-06-15
--------------------------------------------------------------

** Bugfix
	* Bugfix in SNC Command
   
** Modification
	* Change to Version 1.0.007.
	* Internal Links implemented (eg. Link between C/O input and CO-Pilot Output).
	* Tactile Switch functionality implemented for digital Inputs (sends 
	  Unconditional Switch Command with short (<400 ms) or long (>400 ms every 250 ms) keypress).
	* Statusinfo implemented.

Version 1.0.006 - 2016-06-01
--------------------------------------------------------------

** Bugfix
	* Bugfix in pairing routines. 
   
** Modification
	* Change to Version 1.0.006.
	* Heatdemand relay functions on Virt B channels implemented.
	* DEC send to FAL if FAL reset has been detected (sequence counter = 0x01).

Version 1.0.005 - earlier - 2016-05-23
--------------------------------------------------------------

** Bugfix
	* Bugfix in pairing routines.

--- END OF FILE ---