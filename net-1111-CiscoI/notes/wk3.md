### Ethernet framing Wikipedia
<img width="987" height="427" alt="Screenshot 2025-09-02 114952" src="https://github.com/user-attachments/assets/74c304be-9581-4432-85af-dba3936c2233" />

<img width="970" height="522" alt="Screenshot 2025-09-02 115009" src="https://github.com/user-attachments/assets/2d38374a-f4dc-430f-81fc-3c647eed2ae9" />



|Type of ethernet|Purpose|
|------|-----|
|Ethernet II| The Two Octet ethertype field in the ethernet frame preceeded by a destination and a mac address, "Most notably, an EtherType value of 0x0800 indicates that the frame contains an IPv4 datagram, 0x0806 indicates an ARP datagram, and 0x86DD indicates an IPv6 datagram"|
|Novell Raw IEEE 802.3| This ethernet type ran on early IEEE 802.3 framework however it did not use a LLC header, opting to start the IPX packet directly after the length field. This is also unique in that it shouldn't work, but seeing as how Novells' first octet always starts with FF it can peacefully coexist on the wire, thus making this change possible.|
|IEEE 802.3 LLC| More commonly used with large corporations and mainly helps with translating from ethernet to Token Ring and FDDI Networks. There exists a internet policy, though hardly used, for encapsulating IPV4 traffic in IEEE 802.3, however it is used in FDDI networks, Token Rings, and IEEE 802.11, though not on the 5.9 GHz band where Ethertype is used instead.|
|IEEE 802.3 SNAP| The LLC header features two eight bit address fields, when both source and destination are set to 0xAA the LLC header will be followed by a SNAP header. This header allows ethertype values to be used by all IEEE 802 protocols as well as supporting private ID protocol spaces. 

### T568A and T568B differences.
There are two types of Ethernet cable, T568A and T568B. The only difference between the two standards are that the green wires in T568A connect to pins 1 and 2 and the orange connects to pins 3 and 6 whereas in T568B the orange cable connects to pins 1 and 2 and the green wire connects to pins 3 and 6. While more or less the same from a technical standpoint, they are not interchangable. If you use T568A in your home system you must continue to use that T568A for expansion and making a new network. 

### Encoding and framing
Encoding ensures that the bits are transmitted properly, how the bits are managed.
Framing is the process of how the reciever of these bits recieves the packet. When one begins and where it ends. 

### Module 5: Communication

|Protocol of message| Its use|
|---|---|
|Message format| What format is the message in? Formats depend on the channel and the method used to send the message.|
|Message size| Character size can determine if long messages can be sent, or if they should be broken up into smaller segments. Character limit is often determined by the channel.|
|Timing| Timing is how fast a host or reciever can transmit bits. The faster the speed, the more information can be sent.|
|Encoding| messages are sent in bits, bits are converted into electrical impulses, sound waves, or light signals, that can then be converted back into words.|
|encapsulation| encapsulation is the process of including a header that identifies source and reciever information, elsewise the message cannot be sent.|
|message pattern| some messages require acknowledgement when it is recieved before further communication can commence. Some do not.|

Internet standards are a set of rules put in place to determine how something should be done. Internet standards can be ammended in a numbered document called a Request for comments. These are then passed to the Internet Engineering task force though other organizations such as the IEEE and IETF also exist and have their own policies in place.

## Network Communication models
Two main models exist for Network Communication, OSI and TCP/IP. 

TCP/IP is the first internet model made in the early 1970's and is as follows.
|TCP/IP Model Layer|Discription|
|----|----|
|Application| represents data to the user, also functions as encoding and dialog control.|
|Transport| Supports communication between numerous devices across diverse networks|
|Internet| determines the best path through the network|
|Network access| controls the hardware devices and media that make up the network|

|OSI Model Layer|Description|
|-----|------|
|7- Application| Protocols for process-to-process communication.|
|6- Presentation| common representation of data between layers.|
|5- session| helps the presentation layer organize dialog and manage data exchange|
|4- Transport| Segments, transfers and reassembles data for communication between end devices|
|3- Network| exchanges individual pieces of data over the network between end devices.|
|2- data link| exchanges data between devices over a common media|
|1- physical| mechanical, functional, proceedural, and electrical activate, maintain, and de-activate pyshcial connections for a bit transmission to and from a network device.|
