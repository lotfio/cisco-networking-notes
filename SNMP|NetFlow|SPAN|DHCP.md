createdAt: "2018-09-11T13:40:40.432Z"
updatedAt: "2018-09-11T14:18:22.324Z"
type: "MARKDOWN_NOTE"
folder: "06e9f678163ed5819f33"
title: "SNMP/NetFlow/SPAN/DHCP"
content: '''
  # SNMP/NetFlow/SPAN/DHCP
  
  # SNMP
  Remotely monitor the network
  
  * Manager (server)
  * Agent (on devices)
  * TRAPs: information carrier
  * Multiple version
    * V1 (no security, monitor the CPU only)
    * V2c (no security, more features)
    * V3  (more secured, more features)
  
  # NetFlow 
  Controls the netwok flow 
  
  # SPAN
  Sniffs the packets from specefied ports on the current switch & send a copy to a specified port which could contain a server to treat them
  
  
  # RSPAN
  Same as SPAN but works on not direct switch but all the switches
  
  # DHCP snooping
  Only trust one port as a DHCP server for a certain vlan 
  
  ```
  Switch(config)#ip dhcp snooping
  Switch(config)#ip dhcp snooping vlan 1
  Switch(config)#int f0/3
  Switch(config-if)#ip dhcp snooping trust 
  ```
  
  # DAI 
  Dynamic ARP inspection
'''
tags: []
isStarred: false
isTrashed: false
