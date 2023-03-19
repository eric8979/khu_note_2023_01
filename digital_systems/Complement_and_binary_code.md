- mynum : 47
- Contents : chapter 0 ~ 1

## Complements

#### Diminished Radix complement
- (r-1)'s complement of N is ...
            - ((r^n)-1) - N

#### Radix complement
- r's complement of an n-digit number N is ...
	- (r^n) - N  (if N != 0)
	- 0 (if N = 0)

#### Complement for binary
- 1's Complement
	- e.g. 101101 & 010010
- 2's Complement
	- e.g. 101101 & 010011


## Binary code

#### BCD code
- 10 decimal to binary
- 4-bit code for one decimal
- e.g. (185)10 = (0001 1000 0101)BCD
- When addition if sum is greater than 1001, add 0110 to obtain correct BCD.

#### Types
- Weighted code
            - 2 4 2 1
            - Excess-3
            - 8 4 -2 -1
- Self-Complement code
            - 2 4 2 1
            - e.g. 1 (0001) 's complement is 8 (1110).

Q. How computer represents negative int?

### Gray code
- One bit change on a increment.
- Example
	- 0110 == 4
	- 0111 == 5
 - How to make a gray code
 - Method 1
	 - G1
		 - 0, 1
	 - G2
		 - 0 G1, 1 G1^-1
		 - ^-1 means inverse of the gray code
		 - 0 0, 0 1  ,  1 1, 1 0
- Method 2 (Using 8421 code)
	- 8421 -> gray (XOR)
	- copying left first digit and comparing digits using XOR.
	- Example
		- 0111 -> 0100

### ASCII code
e.g. '5' -> ()0110101
- the () is empty. The parity bit
- Even parity
	- Add 0 or 1 to make 1's in the code even.
- Odd parity
	- Add 0 or 1 to make 1's in the code odd.
e.g. 5 -> 00...000101


### Register

### Binary logic