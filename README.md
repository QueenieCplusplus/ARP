# ARP
Router in Ethernet

When a router needs to send a IP packet over an Ethernet Network, router needs to find out what the MAC addr to send the frame(訊框) to.

Given the DES IP, ARP obtains the DES MAC (this may be from Host or from GW Router).

Host got its ARP table with a list realated to IP addr to MAC addr.

# ARP Operation

Router send Broadcast Request. Once if a workstation(its ip addr is 192.168.1.22) has to send a frame or packet to send to 192.168.1.17, however the workstation checks its ARP table, and found out that there is no DES MAC addr in its ARP table.

# Broadcast (a req)

Then the Router broadcasts an APR req to all hosts in the same subnet. The ARP req contains the Sender's IP ,MAC addr and Targets IP addr. (Target MAC addr is wait to be resolve in this phase then)

All nodes in the subnet (the broadcast domain) receive the req and process it (drop or sendback reply).

# Find me out (Unicast)

then the device (host or GW router) with this target IP addr send ARP Reply back to the sender, the msg shows the device's MAC addr. By unicast, the msg sent back to 192.168.1.22. Then the sender got the DES MAC Addr, and learned it, update it to its ARP table using IP addr within relatied MAC addr.
