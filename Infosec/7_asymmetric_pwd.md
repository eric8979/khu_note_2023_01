## Symmetric
- Single key
- Fast
#### AES
	- Chunk the data in to blocks.
	- length
		- IV(128-bits) == block != key(AES-128, AES-192, AES-256)
	- modes
		- ECB
			- Encryption for each block is independent.
			- Same blocks results in same ciphers.
		- CBC
			- block's are dependent with each other.
			- Each block is XORed with the previous ciphertext block before encryption.

---
 
## Asymmetric
- For secure key sharing
- Use two keys for encryption & decryption.

#### RSA
- Utilizes difficulty of **prime factorization**(소인수분해)
- Usage
	- Authentication
	- Digital Signature(전자서명)
		- Proof of ownership on public-key.
			- A encrypts hash value of data using private_key_A.
			- A opens pub_key_A and encrypted data to the public.
			- If the data decrypts to the hash value using pub_key_A, the data is from A.
			- (Someone can change hash value, pub_key, and private_key and claim it's real...
			- (it'll seem legit...)
		- CA (Certificate Authority)
			- Authority encrypt hash value using their private_key
			- Authority opens data, hash_value, and **Digital Certificate**(public_key+)
			- (All the way up to Root CA)
- Mechanism
	- Share pub_key_A and pub_key_B
	- pub_key_A encrypted data can only be opened by private_key_A
	- pub_key_B encrypted data can only be opened by private_key_B
	- Scenario
		- A sends data encrypted in pub_key_B to B.
		- B decrypts the data using private_key_B.

#### Diffie-Hellman
- Usage
	- Key-exchange (K)
- Utilizes difficulty of **discrete logarithm problem**
	- K = pub ^ x mod p
		- Easy : pub, x, p -> K
		- Hard : pub, K, p -> x
- Mechanism
	- p : big prime number
	- g : integer smaller than p (public)
	- Exchange pub_A, pub_B
	- person 1
		- a : private random integer smaller than p
		- pub_A = g ^ a mod p
		- K = pub_B ^ a mod p
	- person 2
		- b : private random integer smaller than p
		- pub_B = g ^ b mod p
		- K = pub_A ^ b mod p
	- Symmetric key **K** generated/shared!
