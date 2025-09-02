### Ethernet framing Wikipedia
<img width="987" height="427" alt="Screenshot 2025-09-02 114952" src="https://github.com/user-attachments/assets/74c304be-9581-4432-85af-dba3936c2233" />

|Type of ethernet|Purpose|
|------|-----|
|Ethernet II| The Two Octet ethertype field in the ethernet frame preceeded by a destination and a mac address, "Most notably, an EtherType value of 0x0800 indicates that the frame contains an IPv4 datagram, 0x0806 indicates an ARP datagram, and 0x86DD indicates an IPv6 datagram"|
|Novell Raw IEEE 802.3| This ethernet type ran on early IEEE 802.3 framework however it did not use a LLC header, opting to start the IPX packet directly after the length field. This is also unique in that it shouldn't work, but seeing as how Novells' first octet always starts with FF it can peacefully coexist on the wire, thus making this change possible.|
|IEEE 802.3 LLC| More commonly used with large corporations and mainly helps with translating from ethernet to Token Ring and FDDI Networks. There exists a internet policy, though hardly used, for encapsulating IPV4 traffic in IEEE 802.3, however it is used in FDDI networks, Token Rings, and IEEE 802.11, though not on the 5.9 GHz band where Ethertype is used instead.|
|IEEE 802.3 SNAP| The LLC header features two eight bit address fields, when both source and destination are set to 0xAA the LLC header will be followed by a SNAP header. This header allows ethertype values to be used by all IEEE 802 protocols as well as supporting private ID protocol spaces. 
