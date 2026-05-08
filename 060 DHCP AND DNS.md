
# Class 06.1: DHCP


```
┌───────┐                       ┌────────┐
│ My PC │          ┌──┬─────────┤  DHCP  │
└───────┴──────────┤SW│         │ SERVER │
                   └──┘         └────────┘
```
### Dynamic Host Configuration Protocol (DHCP)

DHCP automatically hands out IP addresses and other network settings to devices on a network, so you don’t have to configure each one by hand. It streamlines setup, saves time, and cuts down on mistakes caused by manual configuration.

*Alert: The DHCP reservation feature must be disabled for Sonos to work properly.*
<!--! Alert: The DHCP reservation feature must be disabled for Sonos to work properly. -->



There are 4 basic steps DHCP follows to assign an IP address to a device: 

- **DHCP Discover (DHCPDISCOVER) CLIENT**
When a device is first connected to a network, it sends out a broadcast message requesting an IP address. This is a DHCP Discovery message.
- **DHCP Offer (DHCPOFFER) SERVER**
When a DHCP server receives a DHCP Discovery message, it responds with a DHCP Offer message. The Offer message contains an available IP address that the server can assign to the device, as well as other network configuration parameters.
- **DHCP Request (DHCPREQUEST) CLIENT**
The requesting device responds to the DHCP Offer message with a DHCP Request message, indicating that it wants to use the IP address offered by the DHCP server.
- **DHCP Acknowledgment (DHCPACK) SERVER**
Last, the server responds with a DHCP Acknowledgement message, indicating that the device can use the assigned IP address and other network configuration parameters.

(DHCP uses port service: UDP numbers 67 server 68 client)


* ## APIPA (Automatic provisioning of IP Address)
* *When DHCP fails: Link-local is assinged*
* APIPA is (169.254.0.1 to 169.254.255.254) having 65,534 usable IP addresses, with the subnet mask of 255.255.0.0.
* An ip address is always used so PCs on same broadcast domain can comunicate 



### PT activity Configure DHCP on a Wireless Router
<!--! Packet tracer ACTIVITY -->
* Check Files:
* 066 Configure DHCP on a Wireless Router
* 067 simple DHCP





# Class 06.2: DNS


Here’s a quick video explaining how DNS works, from the YouTube channel GetDevOpsReady.
https://www.youtube.com/shorts/h03rYRCrgEA



COMMAND: nslookup


#### Knowledge Check

Which TWO options best describe DNS? (Select 2)
- [ ] A. Translates human‑readable domain names into IP addresses
- [ ] B. Assigns IP addresses automatically to devices on a network
- [ ] C. Allows users to access websites using names instead of numbers
- [ ] D. Identifies devices using a physical hardware address
- [ ] E. Provides wireless connectivity between devices
- [ ] F. Maps IP addresses to MAC addresses on a local network
- [ ] G. Routes traffic between different networks


### PT activity Configure 
<!--! Packet tracer ACTIVITY -->
* Check Files:
* 067 simple DNS v2
