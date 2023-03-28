- All about Optimization

- Three variable map (K-map)
	- Uses gray code
	- If only one literal is different, one gate can be removed.
		- e.g. m0 + m1 = x'y'
		- e.g. m1 + m3 = x'z
  
- 이웃하는 square 를 2^n 묶는다. (bigger the better)
- Draw the squares
	- For square 4 * 4
	- Square size 1, 2, 4, 8(2by4), 16 
	- <--> Literal count in the formula 4, 3, 2, 1(e.g. y'), 0
	- pg. 3, 4, 5

- Prime implicant(주항)
	- Drawing a biggest square possible.
	- The square should not be contained in another square.
	- pg.6 (b) + BD, B'D'
- Essential Prime implicant(필수주항)
	- PI that contains implicant that aren't included in other squares.
- The formula using PI and EPI
	- First write EPIs.
	- Fill in the blanks with regular PIs.