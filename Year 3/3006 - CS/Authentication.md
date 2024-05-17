## What is Authentication?
To allow someone access to an asset we must ensure:
- They are permitted to access that asset
- They are who they say they are
Verification can be done using:
- something the user *is*
- something the user *has*
- something the user *knows*

## Usernames and Passwords
- Identification - who are you?
- Authentication - Verifies that identity
	- Authentication should expire
	- Time of check to time of use (*TOCTTOU*)
		- Repeated authentication
		- At the start & during session

## Problems with Passwords
- People forget them
- They can be guessed
- Spoofing & Phishing
- Compromised password files
- Keylogging
- Weak Passwords (exacerbates the above)

## Weak Passwords
Users have a tendency to use weak passwords:
- spouse, maiden, relative name
- known dates
- Small variants on their own name

|   value    |  occurrence  |
| :--------: | :----------: |
|   123456   | 5.37 × 10^6  |
| 123456789  | 1.96 × 10^6  |
|  password  | 1.16 × 10^6  |
|   qwerty   | 8.70 × 10^5  |
|  12345678  | 77.02 × 10^5 |
|   12345    | 6.78 × 10^5  |
|   123123   | 4.56 × 10^5  |
|   111111   | 4.48 × 10^5  |
|    1234    | 4.43 × 10^5  |
| 1234567890 | 3.97 × 10^5  |
## "Top" Vs. Top

| "Top"                            | Top                      |
| -------------------------------- | ------------------------ |
| Use Antivirus                    | Install Software Updates |
| Use Strong Passwords             | Use *Unique* passwords   |
| Change passwords frequently      | Use 2FA                  |
| Only visit known websites        | Use Strong passwords     |
| Don't share personal information | Use a password manager   |

---

## Hash Functions
A cryptographic primitive that takes a message of any length, and returns a pseudorandom hash of fixed length

$$h(M):\{0,1\}^n -> \{0,1\}^{128}$$
Hash functions are used everywhere. Message authentication, integrity, passwords etc

The output must be indistinguishable from random noise and bit changes must diffused through the entire output
