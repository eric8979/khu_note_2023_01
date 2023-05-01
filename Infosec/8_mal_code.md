- Detecting malicious code
	- Usually uses **hash** value of an already known malicious code.
	- Using behaviour of the code. (Not an easy method)

## Windows PE file
- All executable file
- meta of exe file
- file extension is just a hint for OS
#### Structure
- Header
	- NT Header - Optional Header
		- In the file
			- Address is usually expressed using **base + offset**
		- On memory
			- use Value(which is address on memory)
			- e.g. AddressOfEntryPoint
- Resource
- executable_code(.text section)


## Packing
- 실행압축
- The real `.text` is zipped therefore harder to analyze statically.
- Static analysis
	- Reviewing code without running it.
- Tools
	- UPX
		- for compressing rather than security
	- Themida
		- for security
		- Kakao PC is packed using Themida to protect their code.
		- 가상화기반 난독화(?, virtual machine)


## Obfuscation
- Overcomplicating the code without altering it's function and logic.
- Source code level
	- e.g. Using not well used syntax
	- Not that effective nowadays
- Binary level (assembly)
	- **Basic Block**
		- A chunk of code that is run together
		- check pg.13
	- Control Flow Flattening
		- Hide basic blocks order/relation.
	- Instruction Substitution(overcomplicating)
	- Bogus Control Flow
		- Overcomplicatin statement that only returns True/False
		- Adding code that won't run.
- Tool
	- LLVM Obfuscator