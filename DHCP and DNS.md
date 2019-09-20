# DHCP and DNS
Dynamic Host Configuration Protocol and Domain Name Server

DHCP assigns ip address in a network automatically

**Steps to implement a DHCP Server**
*Only one DHCP server can be implimented for a single network*
1. Create a router and assign it gateway IP address
2. Create a Server (from PCs tab)
3. Goto Configure and assign it's IP address, gatway and dns(optional)
4. Turn on DHCP in settings
5. Add new record add gateway and dns address
6. Configure all clinets to DHCP

**Steps to imlement a DNS Server**
1. Create a server
2. Turn on HTTP/HTTPS
3. Create (optional) and turn on DNS server and then create
4. Add a new record where Host name will be the web address and Address will be the IP address of server where HTTP is server is running