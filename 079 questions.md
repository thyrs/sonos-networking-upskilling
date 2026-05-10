![Alt text](239image-4.png)
__questions__

A user initiates a trouble ticket stating that an external web page is not loading. You detemtine that other resources both internal and external are still reachable. 

Which command can you use to help locate where the issue is in the network path to the external web page:

* [ ] A. ping -t 
* [ ] B. tracert 
* [ ] C. ipconfig/all 
* [ ] D. nslookup 



![Alt text](239image-6.png)
__questions__

A user reports that a company website is not available. The help desk technician issues a tracert command to determine if the server hosting the website is reachable over the network. The output of the command is shown as follows:


```bat 
C:\>tracert 192.168.1.10 
Tracing route to 192.168.1.10 over a maximum of 30 hops: 
1    0 ms  0 ms  1 ms  192.168.5.1       
2    1 ms  0 ms  0 ms  10.0.0.1          
3    *     *     *     Request time out. 
4    1 ms  1 ms  0 ms  10.0.0.2          
5    1 ms  1 ms  0 ms  192.168.1.10      
```

What can you tell from the command output ?

* [ ] A. The server with the address 192.168.1.10 is reachable over the network
* [ ] B. Requests to the web server at 192.168.1.10 are being delayed and time out 
* [ ] C. The Router at hop 3 is not forwarding packets to the IP address 192.168.1.10
* [ ] D. The server address 192.168.1.10 is being blocked by a firewall on the router at 



<!--! PENDING -->


__questions__
Examine the following command output:
C:\Admin>tracert www.cisco.com 
                                                                                                                      
01  <1 ms  <1 ms  <1 ms  2603-6061-943f-72ec-a240-e0ff-fe67-3c14.res6.bia.um [2603:84181:943f:7.:41411:af:67:34141] 
02  13 ms  11 ms  16 ms  2603-9063-0400-01bb-0000-0000-9000-0001.4f16.biainternet.coe [26031063:400:11::11]         
03  17 ms  25 ms  18 ms  lag-61.zb1enc1001h.netops.exchenge.com [24801:044:4000:0:4:111:640]                        
04  16 ms  13 ms  11 ms  lag-29.drtioricev02r.netops.exchangesco. [2001:8:a00:0:4:12:1521]                          
05  •      •      •      Request timed out.                                                                         
06  •      •      •      Request timed out.                                                                         
07  19 ms  18 ms  27 ms  leg-0.pr2.dcal0.netops.provider.com [2001:068:19941:0:4::517]                              
08  21 es  32 ms  23 ms  200114168:1998:0:81:639                                                                    
09  16 ms  15 ms  18 ms  vlsn-103 r10.spine101.1ed03.fah.neter<h.provider.ca. [1600:1408:6401:40b:1]                
10  15 ms  17 ms  22 ms  vlan-110.r03.1ttef101.1m1433.feb.neterch.provider.<me [2400:1408:0400:013::11]             
11  17 es  17 ms  23 ms  vlan-104.r08.tor101.1m103.feb.teterth.mrovider.tme [2600:1408:40b:21011::1]                
12  25 ms  19 ms  19 ms  g2608-1408-c400-038c1•0000-0000-00011-0633.6e9l01.stetic.ot.com [2600:1408:c400:38d::b33]  

Trace complete. 


Which two conclusions can you make from the output of the tracert command (Choose 2) 
Note You will receive partial credit for each correct answer.

* [ ] A. The trace failed after  the fourth hop
* [ ] B. The device sending the trace has IPv6 address 2600:1408:c400:38d:b33 
* [ ] C. The trace successfully reached the www.cisco.com server
* [ ] D. The IPv6 address associated with the www.cisco.com is 2600:1408:c400:38d::b33
* [ ] E. The routers at hops 5 and 6 are offline 




![Alt text](239image-7.png)

__questions__

A network administrator can successfully ping the URL www.cisco.com, but cannot ping a corporate server located at a remote branch in another city.
You need to identify the specific router where packets are being dropped in the path to the remote branch
Which utility should you use? 

* [ ] A. telnet 
* [ ] B. traceroute >> 
* [ ] C. netstat 
* [ ] D. ipconfig 






![Alt text](239image-8.png)

ilegible... jajaja

![Alt text](239image-9.png)




__questions__

look at the picture:
                                                   ┌────────┐
                      ┌─────────┬──────────────────┤INTERNET│
                      │ Router1 │                  └────────┘
                 ┌────┴─────────┴──────┐
            ┌────┴────┐           ┌────┴───┐
            │ Switch1 │           │Switch2 ├───────────┬┬────────┐ 10.0.0.5/16
         ┌──┴─────────┤           └┬───────┤           │File-Srv │    VLAN 10
         │            │            │       │           └┴────────┘
┌────────┼────────────┼───┐   ┌────┼───────┼──────────┐
│    ┌───┴┐     ┌────┬┘   │   │ ┌──┴─┐    ┌┴───┐      │
│    │PC-A│     │PC-B│    │   │ │PC-C│    │PC-D│      │             
│    └────┘     └────┘    │   │ └────┘    └────┘      │
│      172.100.0.0/16     │   │   172.110.0.0/16      │
│         VLAN 100        │   │     VLAN 110          │
└─────────────────────────┘   └───────────────────────┘

While making a configuration change on Router1 a junior technician accidentally reboots the Router1.
Which two statements are true about the impact to communication on the network while the router is temporarly offline (choose 2)

* [ ] A. The file server (File-Srv) can still access the internet 
* [ ] B. None of the PCs can access the file server (File-Srv)
* [ ] C. PC-C and PC-D can still communicate with the file server (File-Srv)
* [ ] D. PC-A and PC-B can still communicate with each other
* [ ] E. PC-A, PC-B, PC-C and PC-D can still communicate with each other


![Alt text](239image-10.png)

__questions__

Which two statements are true about the IPv4 address of the default gateway configured on a host? (Choose 2)
Note You will receive partial credit for each correct selection 

* [ ] A. The same default gateway IPv4 address is configured on each host on the local network,
* [ ] B. Hosts learn the default gateway IPv4 address through router advertisement messages.
* [ ] C. The default gateway is the Loopback interface IPv4 address of the router connected to the same local network as the host
* [ ] D. The default gateway is the IPv4 address of the router interface connected to the same local network as the host
* [ ] E. The IPv4 address of the default gateway must be the first host address in the subnet



![Alt text](239image-11.png)

__questions__

Computers in a small office are unable to access companypro.net. You run the ipconfig command on one of the computers. The results are show in the exhibit. 

You need to determine you can reach the router 

```bat
DHCP enabled............... yes                                 
Autoconfiguration Enabled.. yes                                 
IPv4 Address............... 192.168.0.14 (Preferred)          
Subnet Mask ............... 255.255.255.0                       
Lease Obtained............. Sunday, January 8, 2021 11:00:02 AM 
Lease Expires.............. Sunday, January 8, 2023 12:00:12 PM 
Default Gateway............ 192.168.0.1                         
DHCP Server................ 192.168.0.1                         
DNS Servers0000............ 8.8.8.8                             
                            8.8.4.4                             
NetBIOS over Tcpip......... Enabled                             
```

Which command should you use? 
Complete the command by selecitng the correct options from each drop-down list 

Answer Area 
                        >                           >
|     |            |     |              |
| --- | ---------- | --- | ------------ |
| A.  | traceroute | 1.  | 8.8.8.8      |
| B.  | nslookup   | 2.  | 192.168.0.1  |
| C.  | ipconfig   | 3.  | 192.168.0.14 |
| D.  | ping       | 4.  | 8.8.4.4      |

__questions__

![Alt text](239image-12.png)

You need to determine whether a remote host is reachable through the network 
Which two commands can you use ?
Each correct command is a complete solution. (Choose 2 ) 
Note You will receive partial credit for each correct selection 

* [ ] A. Route print 
* [ ] B. ipconfig 
* [ ] C. Traceroute Or tracert 
* [ ] D. Ping
* [ ] E. Netstat


