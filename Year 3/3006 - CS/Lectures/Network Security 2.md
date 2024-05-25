## Uses of VPNs
Secure connection over unsecure network
- IPSec (network layer)
- TLS (~application layer)
- SSH
- WireGuard


## VPN Service Providers
Not to be confused with VPN service - used for other reasons, not directly related to security
- Bypassing geoblocking
- Avoiding censorship
- Often a simply proxy + vpn

Commercial products, often boast excellent security/ privacy
- in reality, providers see the traffic!
- Need to encrypt before proxy

## Network segmentation
*Dividing* networks into smaller parts.
Granular policies
Damage control, containment
separation can be physical or logical
- distinct routers/ switches
- VLANs
- Software-Defined Networks (SDNs)
- physical resources may be shared but the network is not the same

## Zero trust
In the past, internal networks considered trustworthy
- few restrictions internally
Threats can very much originate from inside the network
- or "lateral" movement if perimeter breached

in a *Zero Trust Architecture*, no implicit trust
- never trust, always verify
- penetrating the perimeter is no longer enough
- it is the current mindset for networks
Explicit and mutual auth, context-aware, attribute/ role based control, least priviledge, segmentation etc

## Common Wi-Fi threats
packet sniffing
rogue access points
password cracking
krack
