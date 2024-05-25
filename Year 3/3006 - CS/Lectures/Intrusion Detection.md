## Anti-Virus
#### Signature-based Detection
- Store some small code signature for each virus
- scan files either in bulk or at runtime, compare with the signatures on file
- Generic signatures
![[Pasted image 20240517162619.png]]
#### Heuristics
- Determine what actions and rules a virus program will normally adopt
- start the program in a VM and see what it does
- Theoretically, could detect a virus that doesn't strictly match a previous signature
- 
#### Machine Learning / Next-Gen
**Anti-Virus**
- File Attributes
- File Contents
- File Heuristics

**NGAV**
- File Attributes
- File Contents
- File Heuristics
- Access Patterns
- Registry Keys
- Configuration
- Network Activity
- System Calls

## Network Attack Models
![[Pasted image 20240517163234.png]]

*Firewalls **DO NOT** protect against attacks using valid protocols or insider machines*

#### Intrusion Detection Prevention
**Intrusion Detection Systems***
- Detects possible intrusion attempts
- Generates alerts and logs for admin

**Intrusion Prevention Systems**
- identical to IDS but also stops the attack

#### IDS Deployment
**Host Base**
- Monitors a *single host* to find suspicious activity including resource/ app usage
- In many ways modern AV does this
- Additional layer of security software running on a host within a protected LAN or VPN
- creates a *profile of usage* for specific users
- Can monitor CPU, memory use, application use and the network stack
**Network Based**
- Monitors *network traffic* and analyse packets from different protocols to identify suspicious activity
- Placed at a *viewpoint on a network* to examine and analyse traffic
	- installed on a firewall or in the DMZ
	- installed behind a screened subnet
- May perform deeper analysis than many firewalls, e.g. stateful protocol analysis and deep packet inspection

#### Components of IDS
**Sensors/ Agents**
- collect and collate data from multiple viewpoints on a network
**Analysers**
- ascertain if an intrusion has taken place
**Reporters**
- notify the admins via alerts on a console or graphical interface

*Multiple sensors allow us to **distribute capture**, but **centralise** computing **overhead***

#### Protocol Analysis
- Hold detailed session information on protocols being used, examine for attacks:
	- why is this user logging in as root?
	- why is this command being sent a 1000 byte buffer as a parameter?
- Computationally costly, and requires the IDS have all possible versions of these protocols described in its database

#### Signature Based Systems
- Like antivirus, signatures are created and stored in a database - operations as well as binaries
- if operations match a defined signature, then an alarm is triggered.
- include some form of attack language
	- mechanisms to describe sequences of events
	- maintain and monitor intermediate states and event transitions

