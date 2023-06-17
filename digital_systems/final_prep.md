## SR latch
![[sr_latch.png]]
- ON S -> light up Q (Q == 1)
- ON R -> light up Q' (Q == 0)

## D latch
![[d_latch.png]]

## Binary Cell
![[binary_cell.png]]
- Basic building block of RAM
- in case of write, select...
	- if input == 0
		- (R == 1, S == 0) --> Reset (Q == 0)
		- 0 is stored!
	- if input == 1
		- (R == 0, S == 1) --> Reset (Q == 1)
		- 1 is stored!

## 4x4 RAM
![[4by4_ram.png]]