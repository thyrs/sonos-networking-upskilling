

# Class 05.1- Number Systems  Comparing the Subnet Mask (how a router works)


## Private Address Range

**Private address ranges** are IP addresses reserved for use **inside local networks**. They are not **routable on the internet** and are reused across many networks.

| Network Address and Prefix | RFC 1918 Private Address Range |
|----------------------------|--------------------------------|
| 10.0.0.0/8                 | 10.0.0.0 - 10.255.255.255      |
| 172.16.0.0/12              | 172.16.0.0 - 172.31.255.255    |
| 192.168.0.0/16             | 192.168.0.0 - 192.168.255.255  |

*ALERT: SONOS devices connect ONLY to Private Address Range networks* 
<!--! ALERT: SONOS devices connect ONLY to Private Address Range networks -->


## IP address network and host portion

### Comparing the Subnet Mask and Prefix Length
```
| Subnet Mask     | 32-bit Address                      | Prefix Length |
|-----------------|-------------------------------------|---------------|
| 255.0.0.0       | 11111111.00000000.00000000.00000000 | /8            |
| 255.255.0.0     | 11111111.11111111.00000000.00000000 | /16           |
| 255.255.255.0   | 11111111.11111111.11111111.00000000 | /24           |
| 255.255.255.128 | 11111111.11111111.11111111.10000000 | /25           |
| 255.255.255.192 | 11111111.11111111.11111111.11000000 | /26           |
| 255.255.255.224 | 11111111.11111111.11111111.11100000 | /27           |
| 255.255.255.240 | 11111111.11111111.11111111.11110000 | /28           |
| 255.255.255.248 | 11111111.11111111.11111111.11111000 | /29           |
| 255.255.255.252 | 11111111.11111111.11111111.11111100 | /30           |
```

### IPv4 addresses 

>  Example 
192.168.2.38/24
|                   |                             |                               |
| ----------------- | --------------------------- | ----------------------------- |
| Network address   | 192.168.2.0                 | reserved                      |
| Broadcast Address | 192.168.2.255               | reserved                      |
| First usable host | 192.168.2.1                 | usually Default-gateway       |
| Last usable host  | 192.168.2.254               | usually the SVI               |
| subnetmask        | 255.255.255.0               |                               |
| usable range      | 192.168.2.1 - 192.168.2.254 | Ip that i can assign to hosts |


### Differentiating networks
By comparing each device’s IP address using an IP calculator, you can accurately determine whether the devices can communicate directly on the same subnet. This avoids confusion caused by network and broadcast addresses. **Here are the simple steps:**

1. Open https://www.calculator.net/ip-subnet-calculator.html and enter the IP address and subnet mask for the first device, then click Calculate.
2. Note the Usable Host IP Range shown in the results.
3. Repeat the calculation for the second IP address using its subnet mask.
4. Compare the Usable Host IP Ranges:
If both IPs fall within the same range → same network
If not → different networks

*Differentiating networks is especially useful in double NAT situations—keep in mind that Sonos devices don’t support double NAT (we’ll cover this later)*
<!--! NOTE: Differentiating networks is especially useful in double NAT situations—keep in mind that Sonos devices don’t support double NAT (we’ll cover this later). -->


### Activity: multiple choice questions

check files:
- 056 Activity numersystems practice.md
- 059 questions quiz
- 



