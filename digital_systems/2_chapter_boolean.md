## Boolean Algebra
- Closure
	- for all a, b ∈ N, if a * b = c and c ∈ N
	- N is **closed** with * operation.
- Associative law
	- (x * y) * z = x * (y * z) 
	- for all x, y, z in S
- Communtative law
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
	- 1 <-> 0
	- `+` <-> *
	- pg.3 (a) is true and (b) is true
	- **DeMorgan**
- Operator precedence
	- Parentheses
	- NOT
	- AND
	- OR

### Boolean functions
- Lots of functions...

#### Definitions
- literal
	- A variable or its complement
- Product-term
	- literal connected by AND
	- Sum of products (SOP)
		- Product-terms connected by OR
	- **minterm**
		- product-term that includes all variables.
		- e.g. x, y, z --> x'yz
		- Canonical sum (canonical SOP)
			- Sum of minterms
- Sum-term
	- literal connected by OR
	- product of sum (POS)
		- Product-terms connected by AND
	- **Maxterm**
		- Sum-terms that includes all variables.
		- Canonical product (POS)
			- Product of maxterms

### Canonical and Standard forms