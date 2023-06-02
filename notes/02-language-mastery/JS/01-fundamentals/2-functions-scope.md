# Key Takeaways

1. Functions
2. Scope

## Functions

It’s important to be aware of the differences between function expressions, arrow functions, and function declarations.

- A function declaration

```js
function greet() {
  console.log(hello)
}
```

A function declaration uses the function keyword, a name, and a function body.

- A function expression

```js
const greet = function () {
  console.log(hello)
}
```

- Arrow function

```js
const greet = () => console.log(hello)
```

## Scope

- Scope refers to where variables can be accessed throughout the program, and is determined by where and how they are declared.

- Blocks are statements that exist within curly braces {}.

- Global scope refers to the context within which variables are accessible to every part of the program.

### Global variables are variables that exist within global scope

Variables that are accessible to any part of the program.

```js
const input = 8
const controlVal = input / 2 + 3

const multiplier = (number, phase) => {
  const val = number * controlVal + phase
  console.log(val)
}
```

There are three global variables in the code above : `input`, `controlVal`, `multiplier`

- Block scope refers to the context within which variables are accessible only within the block they are defined.

### Local variables are variables that exist within block scope

Variable that is defined within a block and only available inside the block

- Global namespace is the space in our code that contains globally scoped information.

### Scope pollution is when too many variables exist in a namespace or variable names are reused

--> defining variables in the block scope is preferable because
global scope can make things like variable collision (using the same variable for two different purposes) more common.