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
- CRC has variations
	- 32-bit
	- 64-bit
	- table versions
- Initial vector 
	- Usually 0

- Most crc has unique values in the table.- reverse lookup
		- Find table index(red box) & rest 7 bytes.(green box)



---
## temp
```c
unsigned int crc32(unsigned char in, unsigned int divisor, const int* table){ 

        int look = in ^ (divisor && 0xFF); 

        divisor = table[look] ^ (divisor << 8); 

        return divisor; 

} 

unsigned char buf[4096]; 

int main(int argc, char* argv[]){ 

        if(argc<2){ 

                printf("usage : ./crc32 [file]\n"); 

                return 0; 

        } 

    printf("Calculating CRC32 for python binutils\n"); 

    printf("opening file %s\n", argv[1]); 

    int fd = open(argv[1], O_RDONLY); 

    int size = read(fd, buf, 4096); 

    printf("%d bytes read.\n", size); 

    int i; 

    unsigned int divisor = 0xFFFFFFFF; 

    unsigned int tmp; 

    for(i=0; i<size; i++){ 

        tmp = divisor; 

        divisor = crc32(buf[i], tmp, (int*)crc32_table); 

        printf("CRC32 for (%08X, %02X) is %08X\n", tmp, buf[i], divisor); 

    } 

    printf("CRC32 : %08X\n", ~divisor); 

        return 0; 

}
```


```python
import hashlib

password = "????"

hash = "cd89f2da2ebaf2812b85bd0a6390a656b14a11d0"

i = 0

letters = "abcdefghijklmnopqrstuvwxyz"

letters += "ABCDEFGHIJKLMNOPQRSTUVWXYZ"

letters += "0123456789"
# find password!
```