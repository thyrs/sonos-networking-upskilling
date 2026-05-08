
# Class 19.1 - More about WIFI

## Wireless technologies:
- **Bluetooth:** Some sonos speaker support bluetooth but initial setup is still shoud be via wifi
- **Celluar broadband:** (LTE) Sonos doesnt support LTE
- **Satellite broadband:** rural areas, expensive (starlink) Sonos doesnt support Satellite internet
- **WIFI:** (regular home use)


## Wireless Networks are classified by their range:
Wireless networks are grouped by how much area they cover. Understanding these categories makes it easier to know what kind of wireless connection is being used and why:

- **WPAN (Wireless Personal Area Network)**  
  Covers a **very small, personal space** around a user. Used for short‑range connections like **Bluetooth** between phones, headphones, or smartwatches.

- **WLAN (Wireless Local Area Network)**  
  Covers a **local area**, such as a **home, office, or school**. This is your typical **Wi‑Fi network** that connects devices to each other and to the internet.

- **WMAN (Wireless Metropolitan Area Network)**  
  Spans a **city or large campus**. Often used by **internet service providers or municipalities** to deliver connectivity across urban areas.

- **WWAN (Wireless Wide Area Network)**  
  Covers **large geographic areas**, such as **regions or countries**. Common examples include **cellular networks (3G, 4G, 5G)** that keep devices connected while moving long distances.


### Activity: sorting
<!--! Activities -->
- check: "093 offline activity"


## Antennas and Devices

- **Omnidirectional antenna**
Sends signal in all directions (360°).
Used in homes and offices.

- **Directional antenna**
Sends signal in one focused direction.
Used for long distance or targeted coverage.


*There is a Wi‑Fi feature that makes a router act like a **directional antenna**.*  
*It’s called **Beamforming**, and it **should be turned off** when using **Sonos devices***
<!--! There is a Wi‑Fi feature that makes a router act like a **directional antenna**.  It’s called **Beamforming**, and it **should be turned off** when using **Sonos devices**. -->



## Wireless access point (WAP) and Extenders
It is important to differentiate between autonomous access points, controller‑based access points, and wireless extenders, and to understand how each interacts with the wireless network. 

**Autonomous Access Point**
Works on its own.
Simple setup, small networks.

**Controller‑based AP (Lightweight AP)**
Managed by a central controller.
Used in large networks (offices, schools).

**Wireless Extender (EXT)**
A device that repeats or boosts Wi‑Fi signal to areas with weak or no coverage.
⚠️ Extenders increase range, not internet speed.

*ALERT: Sonos devices do not support connections through wireless extenders.*
<!--! ALERT: Sonos devices do not support connections through wireless extenders. -->



## Wireless Topologies
Different setups are used depending on whether devices connect directly to each other, through a router, or by sharing a mobile connection.

**Ad hoc mode**
Device‑to‑device connection.
No router. Devices talk directly to each other.

**Infrastructure mode**
Standard home or office Wi‑Fi.
Devices connect through a router / access point.

**Tethering**
Phone as a hotspot.
Your phone shares its internet with other devices.


*Alert: Sonos devices cannot be set up for the first time using tethering or mobile hotspots as the internet connection. Use a regular home Wi‑Fi network for the initial setup.*
<!--! Alert: Sonos devices cannot be set up for the first time using tethering or mobile hotspots as the internet connection. Use a regular home Wi‑Fi network for the initial setup. -->


# Class 19.2 -  WIFI REGULAR WIFI 

## Wifi Topologies blocks

- **Basic Service Set (BSS)**
A __single Wi‑Fi coverage area__ created by __one access point.__

- **Extended Service Set (ESS)**
__Multiple access points__ working together to create __one large Wi‑Fi network.__ Extended Service Sets (ESS)are used in __buildings and campuses__ to provide __one unified Wi‑Fi network__ across large areas


## **802.11 Standards**

Wi‑Fi standards determine the **frequency**, **speed**, and **coverage** of a wireless network.  
There are **two main options** to choose from: **2.4 GHz** and **5 GHz**.

*ALERT:  For some Sonos devices to work, the router must support both 2.4 GHz and 5 GHz.*
*Routers with only 5 GHz are not supported.*
<!--! **ALERT:**  For **some Sonos devices** to work, the router **must support both 2.4 GHz and 5 GHz**.  Routers with **only 5 GHz** are **not supported**. -->


- **2.4 GHz (802.11b)** → **Longer range**  
Here’s the updated version, clean and simple:

Better distance but **slower speeds**.  
Works **better through solid objects** like walls.  
Use **non‑overlapping channels** like **1, 6, and 11** to reduce interference.

- **5 GHz (802.11a)** → **Higher speed**  
Faster performance but **shorter range**.  
Common **non‑overlapping channels** include **36, 40, 44, and 48**.



### **Important settings to check for 2.4 GHz and 5 GHz**
- If both bands (5GHz and 2.4GHz) share the **same Wi‑Fi name (SSID)**, **rename them** and **separate the bands**. Disable Band Steering and Smart Steering if available. 
- Make sure the **wireless mode** is set to **b/g/n** (supports multiple Wi‑Fi standards).
- Set the **channel width** to **20 MHz**.
- **Not all Sonos devices support "Wi‑Fi 5" (802.11ac)**.


## Wireless concepts:

* SSID = wifi wireless name
* Network mode – 2.4GHz or 5.0GHz
* Security mode - security i.e. WEP, WPA, or WPA2.
* Channel settings – frequency bands in use.

### Activity Router simulators 
- check file: "096 Lab Finding wifi features"



# Class 19.3 - Wireless security: 

## WLAN Threats
Wireless networks are **easy to access**, which also makes them **vulnerable to attacks**.  
Understanding common **WLAN threats** helps us understand **which Wi‑Fi settings can interfere with connections and cause connectivity issues**.



**Denial of Service (DoS) Attacks**
  Overwhelms the WLAN with traffic, preventing legitimate users from accessing the network.

**Rogue Access Points (Unauthorized APs)**
  An unauthorized or fake access point that mimics a legitimate one, tricking users into connecting and exposing their data.

**Man‑in‑the‑Middle (MITM) Attack**
  An attacker intercepts communication between a user and the network, allowing data to be monitored or altered without detection.

<!-- ## Shared Key Authentication Methods

* WEP (Wired Equivalent Privacy) > legacy
* WPA (Wi-Fi Protected Access WPA) > Temporal Key Integrity Protocol (TKIP) 
* WPA2 > Advanced Encryption Standard (AES) 
* WPA3 > Protected Management Frames (PMF). -->

## Secure WLANs   
<!-- process with pictures -->
To protect a Wi‑Fi network from __WLAN threats__, several security features can be enabled. Be aware that __some of these features can cause compatibility issues with Sonos__.

- [ ] Hidden SSID / Network Cloaking This a Wi‑Fi feature that controls whether the network name (SSID) is visible. __Sonos doesnt support hidden SSID__

- [ ] **MAC Address Filtering** is a security feature that allows or blocks devices from connecting to a network based on their unique MAC address. If **“block any”** is enabled, it can prevent devices like Sonos from connecting.

- [ ] A VPN (Virtual Private Network) creates a secure tunnel over a public network, such as the internet. For SONOS proper operation, the VPN should be turned off.

- [ ] A **guest network** is a separate Wi‑Fi network created for visitors, isolated from the main network. **Sonos does not work on guest networks.**


*Alert: remember that on supported setups doesnt mean that sono will not work, it may work but it is not guaranteed and it may cause connectivity issues.*
<!--! Alert: remember that on supported setups doesnt mean that sono will not work, it may work but it is not guaranteed and it may cause connectivity issues. -->

<!--! Knowledge Check -->
<!--todo pending: picture... -->
select which wifi attack you can prevent with each security feature:




## Unsupported Setups (Sonos)

These network settings can **break Sonos** or cause **dropouts, missing speakers, or setup failures**.  
If any of these are enabled, **expect problems**.

### **UPnP (Universal Plug and Play)**
Sonos **needs UPnP** to let speakers discover each other and talk on the network.  
If UPnP is off, **devices won’t sync properly**.

### **QoS (Quality of Service)**
QoS tries to “prioritize” traffic but often does a **bad job with real‑time audio**.  
For Sonos, QoS should be **OFF** or it may cause **audio delays and cutouts**.

### **IGMP (Internet Group Management Protocol)**
Sonos relies heavily on **multicast traffic**.
- **IGMP Proxy: OFF** → prevents multicast from being misrouted  
- **IGMP Snooping: ON** → keeps multicast traffic controlled inside the network  
Wrong IGMP settings = **speakers disappear or don’t group correctly**.

### **WiFi Smart Connect**
Smart Connect automatically moves devices between 2.4 GHz and 5 GHz.  
Sonos hates this. It causes **random disconnects**.  
**Turn it OFF.**

### **Airtime Fairness**
Airtime Fairness limits older or slower devices.  
Sonos behaves like a **legacy device** and needs **constant data flow**.  
With Airtime Fairness ON, Sonos gets **throttled** → audio drops.  
**Disable it.**

### **Security & Blocking Features**
Any firewall rule, MAC filter, or “smart security” feature that blocks new devices can **stop Sonos from connecting**.  
If it can block something, **assume it blocks Sonos**—disable it or whitelist Sonos.


*Bottom line:  Sonos works best on a simple, stable network. Fancy router “optimizations” usually make things worse.*
<!--! **Bottom line:**  Sonos works best on a **simple, stable network**. Fancy router “optimizations” usually make things worse. -->



### Activity 
<!--! Sorting Activity -->
- Supported or not 
check file name: "094 offline activity"