- **Lexical analyzer divides stream into tokens.**
- Produce a stream of Names, Keywords, and Punctuation marks from a stream of chars.

- Example
	- Stream of chars
		- x = ( y + 4.0 )  ;
	- Stream of Names/Keywords/Puncutations
		- ID ASSIGN LPAREN ID PLUS ...
	- "Discard white-space and comments."

- Lexical Token : Smallest unit above letter. (Sequence of char)
#### Token Types
- ID
- NUM
- REAL 
	- e.g. 4.37
- IF
- COMMA
- NOTEQ
- LPAREN
- RPAREN

- Reserved words cannot be used as identifiers.

#### Lexer
- Lexical Analyzer
- The first phase of Compilation! (Lexical analysis)
- Turns the Source code into a stream of Tokens.
- How to implement
	- Write from scratch
	- Use Lexical Analyzer Generator
		- Put Regular Expressions in the generator.