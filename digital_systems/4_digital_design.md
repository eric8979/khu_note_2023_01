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