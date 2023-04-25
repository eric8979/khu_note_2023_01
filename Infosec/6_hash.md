- Dynamic input -> Fixed length output
	- e.g. 
		- H(x) = 1
		- H(x) = length(x) % 10 
- Can't reverse the process.
- Has fixed number of possible outputs. (e.g. 128-bit)
- Avalanch effect 
	- Small diff on input makes big diff on output.
- CRC, MD5, SHA1, SHA256, SHA512, ECC

### Hash collision

### Hash crack
- Reversing the function
- Brute-force

### Good Hash
- Avalnch effect
- Collisioin resistance
	- MD5, SHA1 has been cracked...
- Pre-image(reversing) resistance

### Usage
- If I want to know if a downloaded file is content, you can use the hash value to check the purity.
- Encrypting passwords in DB. (with "salt")
- Detecting Integrity of a file
	- e.g. CRC

### Preimage attack(CRC)
- Find a message that has a specific hash value, without having access to the secret key used to compute the hash. (kind of Brute-forcing)
- CRC has variations
	- 32-bit
	- 64-bit
	- table versions
- Initial vector
	- Usually 0

- Most crc has unique values in the table.- reverse lookup
		- Find table index(red box) & rest 7 bytes.(green box)
