

# Class 03.1: Switching concepts (ARP 1st part)

```
      ┌─────────┐
  ┌───┤Switch-01├───┐
  │   └─┬─────┬─┘   │
  │     │     │     │
┌─┴─┐ ┌─┴─┐ ┌─┴─┐ ┌─┴─┐
│PC1│ │PC2│ │PC3│ │PC4│
└───┘ └───┘ └───┘ └───┘
```

1. **Flooding**
- When the swith doesnt know the destination MAC-address, it floods all the interfaces !!with exeption of the incomming interface

2. **MAC-address learning**
- switch learns by ingress mac-address

3. **mac-address-table**
- Switch saves the information on the "mac-address-table" 

4. **how to check basic network information on your PC:** 
- ipconfig /all (windows cmd)
- arp -a (shows ARP table in the windows PC)




### Activity class 03: PT activity
*check file : "PT activity"*
* packet tracers:
* 153 LAB basic configs SW
* 033 verduras
* 148 physical-mode INT-2.9.2 (research if needed)



### QUESTIONS
*check file : 039 questions.md*