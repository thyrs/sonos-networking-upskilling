
# DHCP config
Activity Router simulators 


### choose a Router GUI simulador:
- https://www.tp-link.com/us/support/emulator/ 
- https://demoui.asus.com/
- http://routeremulator.com/
- https://www.snbforums.com/threads/router-ui-emulators.30552/
- https://ui.linksys.com/
- aries, getwgear  

look for the DHCP server config and configure this:

https://ui.linksys.com/ExpertFamily/E3200/1.0.00

###  Configure DHCP services 

network 172.16.254.0/24

    * a. Default Gateway (pool's Default Gateway) ussually .1
    * b. DNS server (8.8.8.8)
    * c. Start IP address: 172.16.254.10 (ussually start at .10)
    * d. Subnet Mask: 255.255.255.0
    * e. Maximum Number of Users (70)
    * f. Save

Take and send SS