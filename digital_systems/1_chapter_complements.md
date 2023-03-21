## Binary number
#### Converting Decimal
- e.g. (0.6875)<sub>10</sub>
0.6875 * 2  = 1 + 0.3750
0.3750 * 2 = 0 + 0.7500
0.7500 * 2 = 1 + 0.5000
0.5000 * 2 = 1 + 0.0000
- Therefore, (0.1011)<sub>2</sub>

#### Converting Octal and Hexa
- (111100000110)<sub>2</sub>
- Octal
	- (111 100 000 110)<sub>2</sub>
	- (  7     4     0     6 )<sub>8</sub>
- Hexadecimal (0 ~ F)
	- (1111 0000 0110)<sub>2</sub>
	- (   F        0      6   )<sub>16</sub>

---

## Complements
- `r` : base of the number system. (2, 10, 8 ...)
 
#### Diminished Radix complement
- (r-1)'s complement of N is ...
	- (r<sup>n</sup>-1) - N
- e.g. (1's complement)
	- (1011000)<sub>2</sub> & (0100111)<sub>2</sub>

#### Radix complement
- r's complement of an n-digit number N is ...
	- r<sup>n</sup> - N  (if N != 0)
	- 0 (if N = 0)
- e.g. (2's complement)
	- (1011000)<sub>2</sub> & (0101000)<sub>2</sub>

## Subtraction
- a - b == a + (-b)
- **Computer stores negative numbers in 2's complement form of same sized positive number.**
	- e.g. +6 (000000110)<sub>2</sub>   -->  -6 (111111010)<sub>2</sub>

- X = 1010100, Y = 1000011
- Using 2's complement...
	- X - Y
		- X = 1010100
		- 2's comp of Y = 0111101
		- sum = 10010001
		- discard end carry if it exists
		- result = - 0010001
	- Y - X
		- Y = 1000011
		- 2's comp of X = 0101100
		- sum = 1101111
		- if no carry, answer is 2's comp of the sum with minus sign attatched
		- result = - 0010001
- Using 1's complement...
	- X - Y
		- X + 1's comp of Y
		- discard end carry if it exists
		- add 1
	- Y - X
		- Y + 1's comp of X
		- if no carry, answer is 1's comp of the sum with minus sign attatched
