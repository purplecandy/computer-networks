## Routing

**Routing is done to help two networks(routers) to communicate with each other**

#### Static Routing
Major parts of routing are
- Network
- Subnet
- Nexthop

*Network*
It's the address of the unkown network

*Subnet*
Subnet mask of the network address

*Nexthop*
Address of the router (gateway) of the mentioned network we are trying to connect.

**Steps to configure static routing are**
1. First assign a new IP address to to the interface the routers are connected.
2. Configure one router and address of the unkown network from other router
3. Repeat it vice-versa to the uknown network's router.
4. Once both routers are configured with their unkown network addresses. Wait for a while and hopefully it should work.

*Command for routing with cli*
`ip route <unkown_network> <unkown_subnet> <its_router_address>`

*Command to delete a routing with cli*
`no ip route <unkown_network> <unkown_subnet> <its_router_address>`

**Steps to configure RIP**
1. First assign a new IP address to the interface of the of the routers.
2. Go to each of the Routers Settings > RIP
3. Add all kown network address to the router
4. Repeat the steps with other routers

*Command to configure a RIP with cli*
```shell
Router>enable
Router#config t
Router(config)# rip
Router(config-if)# network <network_address>
Router(config-if)# exit
```


