## Addressing table

* Configure the following topology
* all devices should ping each other 
* Send screenshot with succesfull ping

| Device    | Interface | IP             | Subnet Mask   |
| --------- | --------- | -------------- | ------------- |
| Zanahoria |           |                |               |
| Apio      |           | 192.168.253.10 | 255.255.255.0 |
| Lechuga   |           | 192.168.253.20 | 255.255.255.0 |
| Tomate    |           |                |               |
| Pepino    |           | 192.168.253.30 | 255.255.255.0 |
| Chile     |           | 192.168.253.40 | 255.255.255.0 |


```https://asciiflow.com/
                                             ┌──────────┐
                                      ┌──────┤ PC Pepino│
┌─────────┐                           │      └──────────┘
│ PC apio ├───────┐                   │
└─────────┘       │ Ethernet port     │ Ethernet port
               ┌──┴─────────┐  ┌──────┴──┐
               │SW Zanahoria├──┤SW Tomate│
               └──┬─────────┘  └──────┬──┘
    Ethernet port │                   │ Ethernet port
┌───────────┐     │                   │     ┌─────────────┐
│ PC Lechuga├─────┘                   └─────┤ Server Chile│
└───────────┘                               └─────────────┘
```
