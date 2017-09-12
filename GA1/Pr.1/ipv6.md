What is /64 in ipv6?

- /64 = von 128 bits sind 64 netz und 64 hosts

- 2 hoch 64 = 18 mal 10 hoch 6

- regel /64 = autoconfig ipv6
-----
What is privacy?

- privacy = hide psysical adress. off for open internet
-----
How to get from physical address to link local?

Example:

physical address: D4 AE 52 32 52 F7

- "FE FF" put in the middle

- D4 AE 52 **FF FE** 32 52 F7

- D4 in dual = D = A 10 B 11 C 12 **D 13**

- 13 IN DUAL = 0000 =0 1000=8 1100=12 **1101=13**

- 4 IN DUAL = 0100 = 4

- D4 IN DUAL = 1101 0100 

- Invert second bit from the right

- 1101 0100 => 1101 0110

- IN HEX = D 6

- D6

- Insert in physical address

- D6 AE 52 FF FE 32 52 F7

- Write in ipv6 syntax

- D6AE:52FF:FE32:52F7

- LINK LOCAL

- Insert FE80

- FE80:D6AE:52FF:FE32:52F7
