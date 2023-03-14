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
- LEXical analyzER
- The first phase of Compilation!
- Scan and identify a finite set of valid tokens that belong to the language in hand.
- Turns the Source code into a stream of Tokens.
- Generates an error if a token is invalid.
- How to build a Lexer
	- Write from scratch
	- Use Lexical Analyzer Generator with regular expressions.
 - Implementing Lexer
	 - Specify each lexical token using [[regular_expression]].
	 - Using regular expression strings, [[finite_automata]] processes input strings and reaches its final state.
