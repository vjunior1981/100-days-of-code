# Annotations day 001

- Installed go using asdf;
- Installed latest version and set it as global;
- Had a problem trying to run `main.go` file:

```bash
go run main.go
compile: version "go1.17.5" does not match go tool version "go1.17.8"
```

- Problem happened because asdf had the old version go env variables;
- Loaded a new shell and everything worked

```bash
go run main.go
Hellow World!
```

- Comments in go are done using two slashes: `//`
- Comparing with a `bash` script structure, you don't need to call a function **after** declaring it.
  - The declaration happens at begin of the script:

```go
package main // declares the main function

import "fmt" // import fmt package to be used

func main() {
	fmt.Println("Hellow World!") // uses the function Println from fmt pkg
}
```

- You can use `/*` for multi line comments:

```go
/*
this
is
multi line
comment
*/
```

- Go has `array` and `slice`. Arrays allow only one data type, while slice allows multiple, but requires more memory;
- We can have a type `map`;
- In golang you have `uint` and `int` types. Use `int` for negative numbers;
- In golang we can have `float32` and `float64`. First for simple precision and second for double;
- Boolean is defined for `bool` word;
- Variables declaration:

```go
// method 1: traditional
var s string = "Hello World"
var i int = 100
var b bool = false
var f float64 = 77.90

// method 2: multiple variables, same type, same line
var s,t string = "foo", "bar"

// method 3: multiple variables, different types
var (
	s string = "foo"
	i int = 5)
)

// method 4: short version
s := "Hello World"

```

- Print variables:

```go
// concat with ,
package main
import "fmt"

func main() {
	var name string = "KodeKloud"
	var user string = "Harry"

	fmt.Println("Welcome to", name, ", ", user)
}
```

- About the Printf - format specifier:
  - `%v` formats the value in a default format;
  - `%d` formats the value in decimal integers;
  - Format specifiers table [here](https://pkg.go.dev/fmt);

- Variable scope:
  - Variables scope are defined in blocks;
  - Inner blocks **can access** variables declared within outer blocks;
  - Outer blocks **cannot access** variables declared within inner blocks;
- Also there are Local vs Global Variables:
  - Local Variables:
    - Declared inside a function or a block;
    - Not accessible outside the function or the block;
    - Can also be declared inside looping and conditional statements;
  - Global Variables:
    - Declared outside of a function or a block;
    - Available throughout the lifetime of a program;
    - Declared at the top of the program outside all functions or blocks;
    - Can be accessed from any part of the program;
- Zero values in golang:
  - If you declare a variable without values, it will assume a default value:
    - For `bool` it will be `false`;
    - For `int` it will be `0`;
    - For `float64` it will be `0.00`;
    - For `string` it will be `""` (empty string);
    - For pointers, functions, etc... it will assume `nil`;


