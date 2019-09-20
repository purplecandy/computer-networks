# Basics of Networking

![Classes](https://tinyurl.com/y6yjy9je)

**Reserved Address**
xx.xx.1.00 - Transferring packets
xx.xx.1.1 - Router Reserved / Default Gateway

 - **Switches don't need any configuration**
-   **Same networks are placed with same network address**
 -  **Communication between two networks with single router doesn't require routing**
  - **Router's interface to be configured to default gateway id. Depending upon the connected to network to that interface.**
- *ping* **command can be used to connection between two devices**

*Command to configure a Router's interface*
```shell
Router>enable
Router#configure terminal
Router(config)#interface FastEthernet0/0
Router(config-if)#ip address 192.168.3.1 255.255.255.0
Router(config-if)#no shutdown
```