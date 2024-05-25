## Windows Security
- Architecture
- Permissions
- Access Tokens
- Authentication

Kerberos protects uni computers

---
## Architecture
![[Pasted image 20240425213709.png]]

---
## Security Subsystem
Runs in user mode

**Local Security Authority** (LSA)
- checks user accounts
- provides access token
- responsible for auditing

**Security Account Manager** (SAM)
- Maintains user account database used by LSA
- Encrypts / hashes passwords

Sam acts like a server, rather than a file

---
## Windows
Predominantly uses *Access Control Lists*

Extends the RWX with:
- take ownership
- change permissions
- delete

32-bit access marks as compared to Unix's 9 bits

Higher degree of control, with associated complexity

---
## Access Control Matrix
Access rights are defined for each combination of subject and object
- quite abstract, but would allow for very fine control
- Not practical, memory requirements bad when scaling
![[Pasted image 20240425214518.png]]

---
## Capabilities
Rather than define the entire set per user, define only the required content
![[Pasted image 20240425214746.png]]

---
## Access Control List
Stored with an object itself, corresponds to a column of an ACM
![[Pasted image 20240425214939.png]]

---
## Access Control
Treats more than just files:
- registry keys
- active directory objects
- groups

Inheritance is implemented 
- file can inherit ACLs from parent directories 