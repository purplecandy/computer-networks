# OSPF
Open Shortest Path First

It's an internet protocal for IP address to find the shortest path to send packets from source to destination.

### How to implment ospf
OSPF implementation is done in the Routers CLI

*Erase all previous configuration and delete all RIP/Static routing*

`router ospf <process_id_int>`
`network <network_address> <wild_card> area <area_no>`

```shell
Router>en
Router#config t
Router(config)#router ospf 1
Router(config-router)#network 192.168.2.0 0.0.0.255 area 0

```
- **process_id**: Process id
- **wild_card**: Complement of subnet
- **area_no**: An integer that defines what level of Area it belongs. Usual it's 0 which represents a backbone area

*Every OSPF netwrok must have area 0*

### Simple OSPF
Simple OSPF is, an OSPF network with only one area i.e 0

### Multi-Area OSPF
Multi Area are similar to connection of different networks separated into different Area lev.l instead of 0. But in order for a Multi Area OSPF to work each level of Area should have a Router path which is connected to a router under Area 0.


