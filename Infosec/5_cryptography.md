### The relation
- CnC server communication encryption
	- For hackers to hide what goes in and out of there Command&Control server.
- Encoding vs Encryption
	- Only encryption uses **KEY**.

- Ransomware

### Encrypted file
- Read in numbers!
- binary file > text file (limited char to print)
- Hexdump
	- Every binary can converted to hexdump
	- e.g. `0x41` (`A` in ascii)
	- If not printable 
		- `.`, `?`, no-print

### Types
- Classic
	- Substitution cipher
		- e.g. Caesar Cipher -> Vigenere
	- Transposition cipher
	- Vuln
		- Frequency analysis (e.g. most used char `e`)
- Modern
	- Symmetric
		- e.g. AES
	- Asymmetric
		- e.g. RSA

### XOR
- bit-wise operation.
- Important in modern encryption. (pg.12)
- base of encoding/encryption.
- Why?
	- L1, L2, L3, L4
	- `A ^ B ^ B = A`
	- XOR SWAP
		- if swap `x` and `y` ...
			- `x ^ y = C`
			- `x` is now... `C ^ x = y`
			- `y` is now... `C ^ y = x`
	- **No Carry propagation** (constant bit length)