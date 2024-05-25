**The Reference Monitor**
- An abstract concept
**The Security Kernel:**
- The implementation of a reference Monitor
**Trusted Computing Base**
- Kernel + other protection measures

*"An Access Control Concept that refers to an abstract machine that mediates all access to objects by subjects"*

#### Placement
- Hardware - dedicated registers for defining privileges
- OS Kernel - eg VM hypervisor 
- OS - Windows Security Reference Monitor
- Service Layer - JVM, .NET
- Application Layer - Firewalls

![[Pasted image 20240425143323.png]]

#### Lower Is Better
- Using an RM or other security feature at a lower level means:
	- We can assure a higher degree of security
	- Usually a simple structure
	- Reduced performance overheads
	- Fewer layer below attack possibilities
- However: 
	- Access control decisions are far removed from applications

#### OS Integrity
- The OS:
	- Arbitrates access requests
	- Is itself a resource that must be accessed
- This is a conflict, we want to use the OS but not mess with it:
	- "Users must not be able to modify the OS"
- Modes of operation
	- Defines which actions are permitted in which mode, e.g. system calls, machine instructions, I/O
- Controlled Invocation
	- Allows us to execute privileged instructions safely, before returning to user code

#### Modes of Operation
- Distinguish between computations done on behalf of:
	- The OS
	- The user
- A status flag within the CPU allows the OS to operate in different modes
![[Pasted image 20240425143933.png]]

Windows & Linux user ring 3 & 0

## Controlled Invocation
- Many Functions are held at kernel level but called from user level code
	- Network & File IO
	- Memory allocation
	- Privileged instructions
- Need a mechanism to transfer between the two rings

#### Interrupts
Exceptions/ Interrupts/ Traps
- the hardware equivalent of a software exception
Handled by an interrupt handler which resolves the issue and returns to the original code
![[Pasted image 20240425165236.png]]
Given an interrupt, the CPU will switch execution to the location given in an interrupt descriptor table

#### Descriptors & Selectors
Descriptors hold information on crucial objects like kernel structure locations
held in descriptor tables
- contain a descriptor privilege level (DPL)
indexed by selectors
- loaded when required
THE CPU protects the kernel by checking the current privilege level (CPL) when a selector is loaded


#### Interrupt Gates
- the code segment (CS) register in x86 has 2 bits reserved for the CPL
- descriptors that have a privilege level higher than where they point are called gates
- since these descriptors are created by the kernel, the offer a secure means of entry into ring 0


