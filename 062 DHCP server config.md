# DHCP SERVER config 
```.txt
             ┌──────┐
             │Router│
             └───┬──┘
┌──────┐         │
│ DHCP │      ┌──┴─┐
│SERVER├──────┤SW01│
└──────┘      └┬───┤
               │   │
      ┌────┐   │   │  ┌────┐
      │PC01├───┘   └──┤PC02│
      └────┘          └────┘
```

### 1 Configure ip and default gateway under > Desktop > ip configuration (DHCP Server)

### 2 Configure DHCP services 
* Services > DHCP > turn it on > Add a diferrent pool name > click Add > speficy:
    * a. Default Gateway (pool's Default Gateway) ussually .1
    * b. DNS server (8.8.8.8)
    * c. Start IP address: 192.168.10.10 (ussually start at .10)
    * d. Subnet Mask 
    * e. Maximum Number of Users (100)
    * f. WCL address (Wireless Lan Controller ip address) -- Optional (if needed)
    * g. Save
### 3. make sure Default pool is all 0000 (zeros)


