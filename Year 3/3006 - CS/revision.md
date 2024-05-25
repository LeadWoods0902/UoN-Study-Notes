## Exam 1
**Question 1: General Computer Security**
a. Give an example of something you are, something you have, and something you know,
with respect to authentication on a computer system. [3 Marks]
b. Define the three components of the CIA model of computer security. For each of these,
name one example of an attack that might seek to break the component. [6 Marks]
c. Explain the strengths and/or weaknesses of the password “football!” if, once hashed, it
is subjected to a brute force and dictionary attack. [5 Marks]
d. Explain DNS Spoofing (DNS Cache Poisoning) attacks. Assuming such an attack was
successful, give two examples of further attacks that could then be mounted. [6 Marks]
**Question 2: Operating Systems and Software Security**
a. What is a “Time of Check to Time of Use” issue? Give an example of a situation where
this might cause a problem. [4 Marks]
b. Explain briefly how controlled invocation, through the use of system calls, is used
within an operating system to restrict access to privileged modes of operation. Why is
this hard for an attacker to circumvent? [5 Marks]
c. Many databases support queries written in SQL. Explain the concept of an SQL injection
attack. What are the possible steps a developer could take to prevent such an attack? [6 Marks]
d. Explain the difference between signature-based, and heuristic-based malware
detection. Suppose an anti-virus package offers only signature-based detection, in
what ways might this pose a security risk? [5 Marks]

## Exam 2
**Question 1: General Computer Security**
a. What is a Permissive (Black Listing) firewall policy? Provide one example of why this
might not always be the best solution. [3 Marks]
b. Data integrity is a core component of the CIA model of computer security. For a
message transmitted over the internet, explain what it means for it to have integrity.
Give an example of a mechanism that enforces this property and describe how it
works. [5 Marks]
c. You have been tasked with securing a database of usernames and passwords. The
passwords are currently stored using the SHA-1 algorithm, without salting. Propose
some improvements to this system and explain your reasoning. [5 Marks]
d. You have been asked by a superior to help protect your corporate network against new
ransomware threats. Discuss what practical steps would you take to make the network as
secure as possible, and prevent damage to assets. Explain your answer. [7 Marks]
**Question 2: Network and Internet Security**
a. What is the main principle behind a denial of service amplification attack? Give an
example of such an attack and outline how it achieves the amplification. [5 Marks]
b. Suppose that a new exploit has been developed that targets a common protocol such
as SSH. Would either a packet filter or application gateway have any chance of being
effective against this? Explain your reasoning. [4 Marks]
c. IP security can operate in either transport or tunnel mode. Briefly explain the
difference between these two modes, including how they affect the structure of the
packets. [5 Marks]
d. During a TLS handshake a server will send a digital signature and a public key
certificate to the client. What security benefit does this part of the protocol provide, and
how? What is an appropriate response from the client if the certificate fails validation? [6 Marks]

## Exam 3
**Question 1: General Computer Security**
a. Someone asks you for advice on the security of one of their accounts, after they’ve
received an email notifying them that their password has been leaked in a security
breach. They log in using a combination of their password, and numeric codes sent to
their phone. Comment on the issues arising from this breach for this user. What would
you advise them to do? [4 Marks]
b. Various recommendations and standards exist that can be considered to represent
baseline security (e.g., Cyber Essentials, the 10 Steps to Cyber Security, and the ISO
27002 Code of Practice). Select two and compare them in terms of their breadth of
coverage and other characteristics you consider relevant. Which would be the most
appropriate for the university to follow and why? [6 Marks]
c. Cryptographic hash functions are used frequently in modern software systems,
including in authentication of users passwords. Explain how hash functions are used to
authenticate passwords, and what benefits hash functions provide in this case. [4 Marks]
d. You have been asked by a superior to help protect your corporate network against new
ransomware threats. Discuss what practical steps would you take to make the network as
secure as possible, and prevent damage to assets. Explain your answer. [6 Marks]

**Question 2: Operating Systems and Software Security**
a. What is a “Time of Check to Time of Use” issue? Give an example of a situation where
this might cause a problem. [4 Marks]
b. Describe in detail the process that occurs when an operating system elevates privileges
to a root or administrator user while executing software. You may use either Windows
User Account Control or Linux Sudo as an example. [5 Marks]
c. What is a zero-day exploit, and why might it pose more of a security concern than a
known exploit? What kind software defence would you recommend against potential zero-
days? Explain your answer. [6 Marks]
d. Explain why permitting execution of code from the stack could be a security concern,
and how an attacker might use this ability. What benefit would preventing execution on
the stack have in this case? [5 Marks]

**Question 3: Network and Internet Security**
a. Describe the differences between the transport and tunnel modes of the Encapsulating
Security Payload in IPSec. [4 Marks]
b. What is the main principle behind a denial of service amplification attack? Give an
example of such an attack, and outline how it achieves the amplification. [5 Marks]
c. During normal use of the internet, it is possible that advertising companies are able to
track user activity on other third party websites. Explain how cookies are used by
companies to achieve this. How might you avoid this? [5 Marks]
d. Your company is considering purchasing an expensive “next generation firewall” that
claims to offer improved performance using application protocol analysis and anomaly
detection. The company currently uses a stateless packet filter to handle incoming
traffic. Discuss potential benefits of this new technology. [6 Marks]

## Exam 4
**Question 1: General Computer Security**
a. Data availability is a core component of the CIA model of computer security. Using an
example of a service running on the Internet, explain the concept of availability. Give
an example of a situation in which new security measures added to this service may
inadvertently affect availability, and explain why. [5 Marks]
b. Traditional password-based authentication has a number of recognised weaknesses due
to the way that users often tend to select and manage them. Identify three examples
of these weaknesses, and indicate the extent to which can be overcome by using
biometric-based authentication instead? What are the potential downsides for
biometrics that passwords do not possess? [5 Marks]
c. Although we would generally advocate that organisations perform risk assessment to
properly understand the threats and vulnerabilities facing their assets, various
safeguards can already be recommended based on the notion of baseline security.
(i) Explain what is meant by baseline security and discuss why it is relevant. [2 marks]
(ii) The lecture series introduced you to three baseline approaches. Select two and
compare them in terms of coverage and any other factors you consider relevant. [6 marks]
(iii) A small retailer in the East Midlands region wants to adopt a baseline approach
that enables them to demonstrate to clients that they take cyber security
seriously. Which of the baseline approaches would you recommend for this
purpose and why? [2 Marks]

**Question 2: Operating Systems and Software Security**
a. In the context of Computer Security, what is a Trojan? How are Trojans usually
delivered to victims, and what advice would you give users on protecting themselves
against these threats? [4 Marks]
b. A security researcher has found a serious vulnerability in a piece of software. They would
like to detail the vulnerability in a talk at a high-profile conference. Explain why a prudent
course of action would be for the researcher to first alert the software developers of the
issue, before disclosing the vulnerability publicly? [4 Marks]
c. Describe the process that occurs when an operating system makes a discretionary
access control decision for a principal performing an operation on an object. You may
use either Windows or Linux as an example. [5 Marks]
d. What security vulnerability exists in the following code? Outline how a hacker would
attempt to exploit it, and what steps the operating system may take to stop them.
int main (int argc, char** argv)
{
char buffer[256];
strcpy(buffer, argv[1]);
return 0;
} [7 Marks]

**Question 3: Network and Internet Security**
a. Explain the issues raised if an attacker was able to obtain persistent session cookies for
other users on a website. How might websites be designed to avoid attacks based on
this? [4 Marks]
b. A computer network uses a signature-based intrusion detection system such as Snort
to monitor network packets for possible attacks. How effective will this system be for
previously unknown threats? What effects, if any, would the pervasive use of
encryption have on the ability of a system like this to function well? [4 Marks]
c. What is the main principle behind a denial of service amplification attack? Give an
example of such an attack and explain in detail how it achieves the amplification.[5 Marks]
d. A recent security event at your organisation has seen every member of staff receive the
same email containing a malware attachment. You have been tasked with the immediate
and longer term responses to this threat. What would you do immediately to limit
potential damage from this attack, and what longer-term steps you might take to
mitigate the risk from attacks similar to this? [7 Marks]