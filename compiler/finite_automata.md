- a.k.a. Finite state machine
- Recognizer for regular expressions.
- A start state ---> One or more final state

### DFA
- Deterministic Finite Automata
- Single output for a single input
- Edges leaving a node are uniquely labeled
- Accept : automation is in a final state
- Reject : No edge to follow (not in a final state)

### NFA
- Nondeterministic Finite Automata
- Conceptual and cannot implemented.
- Used as intermediate step (RE --> NFA --> DFA)
- An edge can be labeled with ϵ (epsilon).


### RE to NFA
![[Pasted image 20230320140208.png]]
- M and N are regular expressions.

### NFA to DFA
- Avoid multiple possibilities(guessing).

#### Basic Functions
- `edge(s,c)`
	- All NFA states reachable from `s` via `c`
- `closure(S)`
	- All reachable NFA states from each s ∈ 𝑆 without consuming any of the input.
	- Similar to `ε closure(P)`
 