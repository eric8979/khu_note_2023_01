### List
- Elements with different types available
- Random access is not allowed.

### Array
- Static
- Single type
- Cannot be assigned, Cannot be returned
	- Name of an array is pointer.
- Always Pass-by-reference
	- Use `const`, when passing as a param.

### Two-dimensional array
- `typedef`
	- to use newely defined array type shortly.

- image error pg.37 - depth should be number of sheets.

### Class
- Use `return` rather than `cout` for reusability.

### Scope resolution operator
`::`
- General
	- To access global variables or functions from within a local scope.
- Implementation file
	- Used before the member functions name to define the functions class.

### namespace
1. `myspace::name`
Use/write everytime for every uses.

2. `using myspace::name`
Declare `myspace::name` for after uses.

3. `using namespacee myspace`
Access every members of `myspace`.

### enum
- e.g. Used to define a set of options.
```cpp
enum Color {
    RED,    // assigned 0
    GREEN,  // assigned 1
    BLUE    // assigned 2
};
```