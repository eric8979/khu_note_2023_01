### Combinational circuit
- input -> output

### Analysis
- truth table -> diagram
- combinational or sequential?
- Obtain output boolean function or the truth table.

### Code conversion
- BCD excess-3
	- decimal + 3 (3 ~ 12)
	- Draw truth table (3~12)
	- Draw box
	- Draw logic diagram

### Binary adder-subtractor
- Half Adder
	- Sum of 2 binary inputs
- Full Adder
	- Sum of 3 binary inputs
	- **Can carry bit from previous addition.**
	- S = x'y'z + xy'z' + xyzA
		- = x'(y'z+y'z') + x(y'z'+yz)
		- = x(y𛲜z)+x(y𛲜z)'
		- = x𛲜(y𛲜z)
		- = (x𛲜y)𛲜z
	- C = xy+xz+yz
		- = xy+x'yz+xy'z
		- = xy + (x'y+zy')z
		- = xy + (x𛲜y)z
  
- Carry lookahead (p.17)
	- Solution for carry delay
		- Carry lookahead generator (p.18, p.19)
	- c0 = 0
	- c1 = a0b0
	- c2 = a1b1 + a0b0(a1𛲜b1)
 
- Binary subtractor
	- Add "M"!
	- "V == 1" : overflow
		- for 8-bit (-128 ~127)
	- underflow
		- floating point
		- Too small factor value (e.g. 2^-1000000000)
		- factor bit size is fixed.
		- Computer treats this as 0 but with a warning.

### BCD Adder
- For addition operation on BCD numbers

### Binary multiplier
- Uses adder

### Magnitude Comparator
- A == B, A < B, A > B

### Decoder
- Fundamental building block in digital electronics.
- Commonly used to select memory addresses, input/output lines, and other control signals based on binary inputs.
- 교재 연습문제 4.25, 4.26

### Encoder

### Multiplexer
- a.k.a MUX
- Passing only a bit from multiple input bits
- Quadruple 2 to 1 line (pg.35)

### HDL 4.12
- Gate level
- Dataflow modeling
	- boolean equation 그대로 표현
- Behavioral modeling