
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

