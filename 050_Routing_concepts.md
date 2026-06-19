
# Class 05.2 Routing Concepts

```
                                          ISP
                          10.0.0.0/24      |
                                ▼          |
                   .1┌──┐ .1           .2┌─┴┐.1
                ┌────┤R1├────────────────┤R2├────┐
                │f0/1└──┘f0/0        f0/0└──┘f0/1│
192.168.20.0/24 |                                │  172.16.20.0/24
                │                                │
               ┌┴──┐.254                      ┌──┴┐ .254
         ┌─────┤SW1├────┐                   ┌─┤SW2├──────┐
         │     └───┘    │                   │ └───┘      │
         │              │                   │            │
       ┌─┴──┐       ┌───┴┐               ┌──┴─┐       ┌──┴─┐
       │PC-A│       │PC-B│               │PC-C│       │PC-D│
       └────┘       └────┘               └────┘       └────┘
         .10          .11                  .10          .11
```

### Routers Segment Broadcast Domains
Here’s the blunt truth: broadcasts are noisy and dumb, and if you let them run wild, they’ll wreck network performance. Switches happily flood broadcasts out every port like they don’t care — because they don’t. Routers, on the other hand, actually do their job. **They stop broadcasts cold**. Every router interface creates a **separate broadcast domain**, and broadcasts stay trapped inside it.

* Switches propagate broadcasts out all interfaces except the interface on which it was received. 
* The only device that stops broadcasts is a __router__.
* Routers __do not__ propagate broadcasts. 
* Each router interface connects to a broadcast domain and broadcasts are only propagated within that specific broadcast domain.


* A problem with a large broadcast domain is that these hosts can generate excessive broadcasts and negatively affect the network.
* The solution is to reduce the size of the network to create smaller broadcast domains in a process called subnetting. 
* Dividing the network address 172.16.0.0 /16 into two subnets of 200 users each: 172.16.0.0 /24 and 172.16.1.0 / 24. 
* Broadcasts are only propagated within the smaller broadcast domains when using subnetting. 

### Activity: PT
*check files:*
055 LAB simple routing lite