# BulbVM Architecture
## Info
- Architecture Generation: 1
- Architecture Codename: Onion
## Technical Specs
- Maximum Supported Sockets: 1
- Maximum Supported Cores: 1
- Maximum Supported Threads: 1
- Maximum RAM: 64 KB
- Maximum Program-Accesible Registers: 16
## Registers
### Program Accesible
There are up to 16 program-accesible registers, numbered from 0x0 to 0xf in hexadecimal. Onion will have 8 program-accessible registers. Unless specified below, each
register is a general-purpose register.
- PC (0x0): Program Counter
- AC (0x1): Accumulator
- SP (0x2): Stack Pointer
- FLAGS (0x3): Flags Register
- A (0x4)
- B (0x5)
- C (0x6)
- D (0x7)
### FLAGS REgister
Like other registers, FLAGS is 16 bits wide and can be written to by programs. However, only 5 bits are used, and each tells the system whether something was true or
false last time the computer checked. The flags are:
- CARRY (1st bit): Tells whether an arithmetic or SHIFT operation has a bit outside the data's range.
- ZERO (2nd bit): Tells whether the last operation resulted in zero.
- MRTHN (3rd bit): Tells whether a CMP operation resulted in the first value was greater than the second.
- LSTHN (4th bit): Tells whether a CMP operation resulted in the first value was less than than the second.
- EQUAL (5th bit): Tells whether a CMP operation resulted in the first value was equal to the second.
## Instruction Set
### Jargon
- The first 8 bits of the RAM unit are referred to as the 'instruction'.
- The next 4 bits are referred to as 'data unit 1'.
- The next four bits are referred to as 'data unit 2'.
- The next RAM unit in RAM is referred to in some instructions as 'RAM Data'.
### Instructions
-To Be Added-
