## IP Security
Ip is connectionless and stateless
- best effort service
- no delivery guarantee
- no order guarantee
- all above provided by TCP
IPV4 has no guaranteed security suport


## IPSec
Optional in IPv4, mandatory in IPv6
Two major security mechanisms
- IP Authentication Header (AH)
- IP **Encapsulation Security Payload** (ESP)
Does not contain any mechanisms to prevent traffic analysis

## Encapsulation Security Payload
Includes an additional header within the IP packet that describes what encryption and authentication is in use.

![[Pasted image 20240518214529.png]]

## Security Parameter Index
Stores security parameters e.g. crypto protocol keys
Established by internet security association and key management protocol (ISAKMP) during **Internet Key Exchange** (IKE) handshake
Uses *Diffie-Hellman* for key exchange
The SPI references the entry in a table that corresponds to this session's parameters

## ESP in Transport Mode
![[Pasted image 20240518214922.png]]

## ESP in Tunnel Mode
![[Pasted image 20240518220003.png]]
## ARP
a protocol used in IPv4 to obtain mac addresses for given IPs
- used prior to constructing IP and TCP packets for communication
- Network layer

![[Pasted image 20240518220841.png]]

## ARP Cache Poisoning
send an unrequested ARP reply, overwriting the MAC address in a hosts ARP cache with our own.

![[Pasted image 20240518221152.png]]

## ARP protection
Some OSes **ignore unsolicited ARP requests**, or can be configured to use ARP differently
Some software, such as **intrusion detection** packages, will include ARP spoofing detection
- Maintain a log of current MAC:IP assignments and ARP requests/ replies
- Allows us to spot suspicious messages such as unsolicited ARP replies

## DNS
translates domain names into IP addresses
e.g. nottingham.ac.uk -> 128.243.80.167

DNS packets are UDP
- stateless, on the transport layer

DNS resolvers will cache the IPs for a while

![[Pasted image 20240518221633.png]]

 