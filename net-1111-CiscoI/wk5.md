# TCP/IP layer

![The thing](https://github.com/user-attachments/assets/14969533-2edb-4b21-8257-5530245f7926)

the application layer deals with making data, typically in HTTP

The data then gets passed to the transfer layer, passing the data through. This can be done in TCP and UDP

The intranetwork segment then creates the packet and adds its header to the existing data packet and the transfer header.

The network access layer encapsulates the header in a header and trailer depending on the network access type and sends the whole packet along its way. 


The OSI layer is a bit more detailed, however the TCP/IP layer is the main architechture people use and have been using for fifty years. 


# Application: Handles the following functions 

Access by applications to network services

Client/server data access

Name resolution

Dynamic address assignment


# Lab 1 day 2
IPv4 addresses are private IP addresses that are reserved for internal networks and not through the internet. 

Subnet masks are used to determine the range of IP addresses in the same subnet.

any subnet outside the range will require a default gateway.

IPv6 addresses that start with fe80 are link-local addresses which has to be self assigned. 

# DHCP
DHCP is a Dynamic Host Configuration Protocol, given a list of available IP addresses it can help manage devices and their Ips over a large network. 

Reservations in a DHCP are used to give a IP address to a spesific MAC address as each NIC card is given its own unique MAC address, it can be sure to only give a spesific IP address to a spesific Mac address.

Exclusions remove spesific IP addresses from the pool of addresses that can be given out. such as having a range of numbers from 1 to 10 and removing numbers 4, 7, and 9.

Lease times can be issued to only allow an IP address to stay with a computer for a certain time frame, from a few minutes to an indefinite period of time, thus allowing the IP to be returned to the pool and allowing it to be given to a new device.



Authentication/user logon

Data formatting and translation

# data transfer
