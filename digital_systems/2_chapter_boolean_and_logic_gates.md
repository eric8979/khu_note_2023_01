## Theorems and Algebra
- Closure
	- for all a, b ∈ N, if a * b = c and c ∈ N
	- N is **closed** with * operation.
- Associative law
	- (x * y) * z = x * (y * z) 
	- for all x, y, z in S
- Commutative law
	- x * y = y * x
	- for all x, y in S
- Identity element
	- for all x ∈ S, e * x = x * e = x
	- e is identity element.
	- e.g. 1 in multiplication, 0 in summation
- Inverse
	- for x, y ∈ S  if x * y = e
- Distributive law
	- x * ( y + z ) = x * y + x * z
- **Duality** (쌍대성)
	- x + x = x
	- x * x = x
	- **DeMorgan**
		- (x + y)' = x'y'
		- (xy)' = x' + y'
	- pg.3 (a)'s' are true and (b)'s are true.
		- 1 <-> 0
		- `+` <-> *
- Operator precedence
	- Parentheses
	- NOT
	- AND
	- OR

### Functions
- e.g. F<sub>1</sub>  = x + y'z

---

### Definitions
- Literal
	- A variable or its complement
- Product-term
	- Literals connected by AND
	- Sum of products (SOP)
		- Product-terms connected by OR
	- **min-term** (m)
		- product-term that includes all variables.
		- e.g. x, y, z --> x'yz
	- Canonical sum (Canonical SOP)
		- Sum of minterms
- Sum-term
	- literal connected by OR
	- product of sum (POS)
		- Product-terms connected by AND
	- **Max-term** (M)
		- Sum-terms that includes all variables.
	- Canonical product (Canonical POS)
		- Product of maxterms

---

### Canonical
- x, y, z truth table
	- Check ch.2 pg. 7
- Function examples
	- f<sub>1</sub> (for x, y, z)
		- result : 01001001 
	- min-term expression
		- f<sub>1</sub> = x'y'z + xy'z'+ xyz = m<sub>1</sub> + m<sub>4</sub> + m<sub>7</sub> = ∑(1, 4, 7)
		- Numbers for m's are the location of 1's in the table
	- Max-term
		- f<sub>1</sub> = (x+y+z)(x+y'+z)(...) = M<sub>0</sub>M<sub>2</sub>M<sub>3</sub>M<sub>5</sub>M<sub>6</sub> = ∏(0, 2, 3, 5, 6)
		- Numbers for M's are the location of 0's in the table
	- F = xy + x'z
		- result : 01010011
		- F(x, y, z) = ∑(1, 3, 6, 7)
		- F(x, y, z) = ∏(0, 2, 4, 5)
		- This can be produced using...
			- Truth Table
			- Logical Algebra by changing the form of a formula. (Use the algebra)

### Standard forms
- Sum of product
- Product of sum
- Less levels == low delay
	- EX) (b) is better than (a)

### More logical operations
- NOR 
	- x ↓ y = (x + y)'
- NAND 
	- x ↑ y = (xy)'
- XOR 
	- x 𛲜 y = xy' + x'y
- Equivalence
	- (x 𛲜 y)' = xy + x'y'
- ...

### Digital logic gates
- Check ch.2 pg.15, 16

- NAND and NOR operation are not associative.
	- e.g. (x↓y)↓z != x↓(y↓z)
	- Resolve by using 3 or more inputs
		- e.g. x↓y↓z= (x+y+z)'
		- e.g. x↑y↑z= (xyz)'
- XOR is  associative

- Positive logic and Negative logic


### Integrated Circuits (2.9 pptx)
- VLSI
	- Very large scale integration(millions of gates)
	- e.g. complex microcomputer chips
- CMOS
	- Recently used for VLSI design
- Params of a gate
	- Fan-out : Load a output can handle.
	- Fan-in : Number of inputs available in a gate.
- ASIC 
	- Application-specific Integrated Circuit
	- e.g. Camera chip
- **FPGA**
	- Field programmable gate array
	- IC designed to be configured by a customer or a designer after manufacturing