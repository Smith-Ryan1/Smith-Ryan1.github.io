# Binary for dummies
Binary, much like everything with IP addressing it seems, is read as an octet, that is eight sequential numbers, all ones and zeros. Binary is read from powers, the first number (or the last if reading left to right) is 1, then 2, then four. Doubling each time to 128. 255 being 11111111, 64 being 01000000 etc. etc.

# casting types of ipv4 addresses, their subnets and their binaries.
Unicast: casting unilly, one device to one device at a time. Subnet= 255.255.255.0 11111111.11111111.11111111.00000000


Broadcast: one central device, casting to all devices on a network. Cable tv broadcasting to all tvs on its service. subnet 255.255.255.255 11111111.11111111.11111111.11111111

Multicast: like broadcast but only to subscribed multicast devices. subnet range of 224.0.0.0 to 239.255.255.255 01111100.00000000.00000000.00000000 to 11101111.11111111.11111111.11111111

# Private networks

|Ip address/ length| Range of addresses| Binary|
|---|---|---|
|10.0.0.0/8| 10.0.0.0-10.255.255.255| 00001010.00000000.00000000.00000000 - 00001010.11111111.11111111.11111111|
|172.16.0.0/12| 172.16.0.0- 172.31.255.255| 10101100.00010000.00000000.00000000 - 10101100.00011111.11111111.11111111|
|192.168.0.0/16| 192.168.0.0 - 192.168.255.255| 11000000.10101000.00000000.00000000 - 11000000.10101000.11111111.11111111|

Private IPv4 addresses are used for internal use, such as in a large company. Should a Private Network computer wish to send packets globally they would have to have their IP translated into a public IP address before routing. This is done using a NAT (Network Address Translation) and can be done via a router that does connect to the public internet. 

# Special use IP addresses

Loopback addresses: 127.0.0.0 to 127.255.255.254 (but are more commonly addressed as 127.0.0.1) This IP is used to direct traffic from a host back to itself, the ping command is an example of how it could be used to test the connectivity of devices.

Link-Local addresses: 169.254.0.1 to 169.254.255.254 more commonly reffered to as Automatic Private IP Addressing, they are used by windows clients to self configure in the event an IP cannot be found by any other means.

# Legacy IP Classful classification

|Class| IP range| Description|
|----|----|----|
|A| 0.0.0.0/8 to 127.0.0.0/8| Used in very large networks with 16 million host computers. It emplyed a fixed /8 prefix with the first octet to name the network, and the remaining octets were used as host ip addresses.|
|B| 128.0.0.0 /16 - 191.255.0.0 /16| Designed for a network of about 65 thousand hosts. The two high order octets were set to hold the network address while the two lower held the IP.|
|C| 192.0.0.0 /24 - 223.255.255.0 /24| Designed for a small network of only 254 devices. the first three octets held the network address while the last octet held the IP|



