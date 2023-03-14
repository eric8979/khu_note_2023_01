- mynum : 47
chapter 0 ~ 1

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