
# Class 08.1 
## class network ports: TCP vs. UDP

**Network ports** are like rooms inside a building. The building has **one address (IP address)**, but each room **(port number)** offers a **different service**. Let’s explore some of the **most common ports used by Sonos systems**.

<!-- 
* 0 - 1023 Well-know Ports
* 1024 - 49151 Registered Ports
* 49152 - 65535 Private Dynamic ports
-->


### common ports for SONOS:

- 80, 443 (TCP) Content services, radio, and Sonos account
- 445, 3445 (TCP) Music library
- 1400, 1410, 1443, 1843, 3400, 3401, 3500 (TCP) Sonos control
- 4070 (TCP) Spotify Connect
- 4444 (TCP) System updates
- 7000 (TCP) AirPlay
- 136–139 (UDP) Music library
- 1900, 1901 (UDP) Sonos app control
- 2869, 10243, 10280–10284 (UDP) Windows Media Sharing
- 5353 (UDP) Spotify Connect
- 6969 (UDP) Sonos setup


*Alert: The ports used by Sonos must be allowed on the network router (FIREWALL) for the system to work properly.*
*For more information on the ports Sonos uses, see this article:*
*https://support.sonos.com/en-us/article/configure-your-firewall-to-work-with-sonos*
<!--! Alert: The ports used by Sonos must be allowed on the network router for the system to work properly. For more information on the ports Sonos uses, see this article: https://support.sonos.com/en-us/article/configure-your-firewall-to-work-with-sonos -->




# Class 08.1 TCP vs. UDP

**TCP and UDP** are transport‑layer protocols that control how data is sent between devices. **TCP** prioritizes reliability and order, while **UDP** prioritizes speed and low latency, making each suitable for different types of network traffic.

| Feature          | TCP                                | UDP                                  |
| ---------------- | ---------------------------------- | ------------------------------------ |
| Connection type  | Connection‑oriented                | Connectionless                       |
| Reliability      | Reliable (guarantees delivery)     | Unreliable (no delivery guarantee)   |
| Order of data    | Data arrives in order              | Data may arrive out of order         |
| Speed            | Slower (more overhead)             | Faster (less overhead)               |
| Error checking   | Error checking: Yes                | Error checking: Minimal              |
| Best used when   | Accuracy matters more than speed   | Speed matters more than accuracy     |
| Common use cases | Web browsing, file transfer, email | Streaming, voice, discovery services |


### PT Activity - 
<!--! PT Activity - unblock / block ports on wireless router -->
- check file: "085 lab PT ports"