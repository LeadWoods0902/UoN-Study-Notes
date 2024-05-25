## Authentication Factors
#### What are factors?
something the user *is*
something the user *has*
something the user *knows*

## Inherence factors (Biometrics)
- Unique identifiable biological characteristics
- Distinctly inherent to an individual

#### Example Systems:
- Fingerprints 
- Facial
- Iris 
- Vocal
- Behavioural
	- Dynamics (mouse, keyboard use)
	- Gait, Posture
	- Usage Patterns


#### Biometric Authentication Process
![[Pasted image 20240425135548.png]]

#### Pros & Cons
| Pros                     | Cons                             |
| ------------------------ | -------------------------------- |
| No Risk of Losing Access | Availability/ Cost/ Requirements |
| Very Convenient          | Errors                           |
|                          | Can never be changed             |
|                          | Not Foolproof                    |
|                          | Ethical/ Privacy Concerns        |
 
## Possession Factors (Hardware Tokens)
#### USB Tokens
- Keys
- Card Readers
#### Smart Cards
- Metal Contacts / RFID
- Access Control, Public Transport, Banking
#### Personal Device
- Phone/ Watch
- Readily Available
- Often a *single point of failure*
#### FIDO/ WebAuthn
![[Pasted image 20240425140703.png]]
#### Pros/ Cons
| Pros                                 | Cons                         |
| ------------------------------------ | ---------------------------- |
| Relies on Strong Keys & cryptography | Physical loss, damage, theft |
| in Principle very strong             | Cost                         |
|                                      | Usability                    |

## Knowledge Factors (Passwords)
- Prone to be guessed, cracked, stolen, misused
- Often the weakest link
- Still not well managed
- Much effort to replace


## Managing Passwords
Single Master Password Vs Many Passwords
- Entropy sufficient for individual "service" passwords
- Entropy better since a single password is needed
Convenience
- Centralized
- Autofill
Not all free
Master Password is a single point of failure
- Attractive target
- Still requires good password hygiene
Vaults still at risk
- Leaks
- Can you trust a single third-party with all your auth data
Trading some types of attacks
- service leaks/ mismanagements
- Lower Entropy
... against others
- vault leaks
- malware
- bugs

## Authentication Characteristics
![[Pasted image 20240425141803.png]]

## MFA