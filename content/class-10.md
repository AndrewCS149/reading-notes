# JS Error Handling and Debugging

---

#### Scope

Functions have **lexical scope**. This means that a functions are linked to the objects (or functions) they are defined inside of.

#### Errors

Javascript throws an **exception** when a statement fails to execute. The interpreter will then look for an exception-handling code and return an **exception-object**. Examples:

- `Error:` Generic error
- `SyntaxError:` Invalid syntax
- `ReferenceError:` No variable found
- `TypeError:` Wrong data type used
- `RangeError:` Number outside of given range
- `URIError`
- `EvalError`

Dealing with errors can be done with a ```try catch throw or finally``` statements.

---

#### Debugging Workflow

It is important to debug code methodically.

1. Identify the location of the bug
   1. The error message should describe the cause and location of the bug
   2. Figure out how far the script runs before breaking (console.log() can be helpful)
   3. Use breakpoints at the location of the bug
2. Identify the cause of the bug
   1. Set breakpoint and see if the variables hold the correct value
   2. Deconstruct the code into smaller pieces and see check which values each variable is holding, if an object has been constructed, etc.
   3. Check the parameter of a function

The chrome dev tools is a great way to help debug code.

