## Flashing Netgear stock firmware to DD-WRT

![Log](https://webobjects2.cdw.com/is/image/CDW/2192921?$product-main$)
 
__Router Name : Netgear  N600 Dual Band Router__  
__Router Model : WNDR3400v2__
 
Stock firmwares that comes usually with many routers are limiting in terms of creating multiple SSIDs and VLANs. Therefore, to be able to control the network properly and use the advanced features of segmentation and privacy, an advanced firmware is needed.
 
 
Why DD-WRT?
 
DD-WRT is an open source firmware that offers advanced features:
 
Multiple SSIDs : can be used to isolate the network into separated subnets
VLANs: Virtual Local Area Network allows the separation of ports. Each port in the router or switch can be isolated from the rest of the ports
IPtables Firewall
OpenVPN, PPTP, & L2TP VPN Client/Server Integration
 
 
Note: There are ready routers with DD-WRT install on them. However; if you have an old router  that is compatible with DD-WRT would good to flash it and use it instead purchasing one 
 
5 steps to flash the router
 
1- Make sure the router is compatible with DD-WRT to avoid bricking issues
 
Check DD-WRT database to  check the model number and its version 
 
DD-WRT Router Database : https://www.dd-wrt.com/site/support/router-database
 
 
2- Hard Rest :
 
If the router is compatible with DD-WRT. Proceed with hard reset known as  30/30/30
 
Hold the reset button at the back of the router for 30 seconds
Then unplug the router for 30 seconds while holding the reset button 
Plug the router back and continue holding for 30 seconds
 
Note: do not release the reset button until you finish the 120 seconds in order
 
3- Updating the router firmware
 
Access the Default Gateway address of the network, usually for Netgear routers are 192.168.1.1 and enter the username and password
 
Go to Advanced section of the settings under Administration → Router Update 
	
 
Upload the firmware and wait for it until it completes the process
 
For this router model DD-WRT do not have a firmware on its database. Netgear Open router community provides the DD-WRT for this version
	
	Netgear open router community : https://www.myopenrouter.com/
 
The build is uploaded to the resources section of this repo
 

 
Note: the router at this stage will turn on and off multiple times during the flashing time
 
 
4-  DD-WRT Web GUI
 
If the firmware is installed correctly, you should see the below web gui
 

		
 
 
Pros and Cons of this this build of DD-WRT
Pros:
 
Can have multiple SSIDs
 
Cons:
Does not support network encryptions : WPA,WPA2
It works only on Open networks
 
 
 
 
