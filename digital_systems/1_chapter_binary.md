## Signed binary
- +9 == (0 001001)<sub>2</sub>
- Signed magnitude representation
	- -9 == (1 0001001)<sub>2</sub>
- Signed complement representation
	- 1's : (1 110110)<sub>2</sub>
	- 2's : (1 110111)<sub>2</sub>
- Summation and Subtraction
	- Signed magnitude system follows ordinary arithmetic.
	- 2's Signed complement system requires only addition.

---

## Binary code
#### BCD code
- 10 decimal to binary
- 4-bit code for one decimal
- e.g. (185)<sub>10</sub> = (0001 1000 0101)<sub>BCD</sub>
- When addition if sum is greater than 1001, add 0110<sub>2</sub> (or 6) to obtain correct BCD.
- Usage
	- To make it simpler for machine to understand human readable numbers.

#### Types
- Weighted code
	- 2 4 2 1
	- 8 4 -2 -1
- Non-weighted code
	- Excess-3 : BCD + 0011
	- Gray code
  
- Self-Complement code
            - 2 4 2 1
            - e.g. 1 (0001) 's complement is 8 (1110).

### Gray code
- Only one bit change on a increment.
- Good for error detecting.
- Example
	- 0010 == 3
	- 0110 == 4
	- 0111 == 5
 - **How to make gray code**
 - Method 1
	 - G1
		 - 0, 1
	 - G2
		 - 0 G1, 1 G1<sup>-1</sup>
		 - -1 means inverse of the gray code
		 - 0 0, 0 1  ,  1 1, 1 0
- Method 2 (Using 8421 code)
	- 8421 -> gray (XOR)
	- copying left first digit and comparing digits using XOR.
	- Example
		- 0111 -> 0100

### ASCII code
e.g. '5' -> ()0110101
- the () is empty. The parity bit(error detection)
- Even parity
	- Add 0 or 1 to make 1's in the code EVEN.
- Odd parity
	- Add 0 or 1 to make 1's in the code ODD.
e.g. 5 -> 00...000101

### Register

### Binary logic
- AND
- OR
- NOT