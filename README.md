# ARP
Router in Ethernet

When a router needs to send a IP packet over an Ethernet Network, router needs to find out what the MAC addr to send the frame(訊框) to.

Given the DES IP, ARP obtains the DES MAC (this may be from Host or from GW Router).

Host got its ARP table with a list realated to IP addr to MAC addr.

# ARP Operation

Router send Broadcast Request. Once if a workstation(its ip addr is 192.168.1.22) has to send a frame or packet to send to 192.168.1.17, however the workstation checks its ARP table, and found out that there is no DES MAC addr in its ARP table.
