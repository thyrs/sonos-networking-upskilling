
# Class 02.1 Media Types 


### Network interference

**EMI: ElectroMagnetic Interference:** Electromagnetic interference (EMI) is unwanted noise or disruption in an network caused by external electromagnetic fields, which can degrade the performance of electronic devices or even cause them to malfunction.

**RFI: Radio Frequency Interference**
Radio Frequency Interference  (RFI) is a subset of EMI specifically dealing with high-frequency disturbances in the radio frequency spectrum



## Three Media Types


### __Metal wires within cables__ - Data is encoded into electrical impulses.

- __Twisted-Pair Cable__:
 * Cable de Red: RJ45 cable connector(Ethernet cable)
* RJ-11 Cable (telefono)
![Alt text](144image.png)


### __Coaxial Cable__
![Alt text](144image-1.png)

### __Glass or plastic fibers within cables__ 
  * large distance
  * Expensive 
  * (fiber-optic cable) - Data is encoded into pulses of light.
    ![023_Fiber.jpg](143_Fiber.jpg)
    
### Wireless transmission - Data is encoded via modulation of specific frequencies of electromagnetic waves.
* WIFI (802.11)


### Activity class 02: problem - solucion
<!--! Activity class 02 -->
*check file : "026 Sorting Activity"*


# Class2.2 - IP Address and MAC Address 

In network communication, devices are identified using two types of addresses: a logical address (IP address), used for routing across networks, and a physical address (MAC address), used for communication within a local network.

**MAC address**
A MAC address is typically formatted using letters from A–F and numbers from 0–9, written as 12 hexadecimal characters, usually shown as 6 pairs separated by colons or hyphens, for example: 00:1A:2B:3C:4D:5E.

**IPv4 address**
An IPv4 address is formatted as four numbers ranging from 0 to 255, separated by dots, for example: 192.168.1.1.
kahoot:

### Activity class 02: 029 questions
*check file : "029 questions"*
<!--! class activity simple questions.-->




# Class 2.2 - Unicast Multicast Broadcast 


### Unicast MAC Address (one to one)
![Alt text](161image-2.png)


### Multicast MAC Address (one to some)
There is a destination MAC address of 01-00-5E when the encapsulated data is an IPv4 multicast packet and a destination MAC address of 33-33 when the encapsulated data is an IPv6 multicast packet.

The range of IPv4 multicast addresses is __224.0.0.0__ to 239.255.255.255. The range of IPv6 multicast addresses begins with ff00::/8.

![Alt text](161image-4.png)

### Broadcast MAC Address (one to all)

![Alt text](161image-3.png)


--

*Multicast needs to be enabled on the network for Sonos devices to function properly.*
<!--! Multicast needs to be enabled on the network for Sonos devices to function properly. -->


### Activity class 02: PT activity
*check file : "PT activity"*
* packet tracers:
* 023 Lab media
* 023 LAB_IoT
* 027 physical-mode INT-2.9.2 (research if needed)
    - to remove cable take it from the head of the cable and put it back in the cable pegbard
    - u should get around 50% (take SS)
