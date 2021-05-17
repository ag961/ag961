# Chapter 10: Error Handling and Debugging

Source:
> Duckett, J. (2014). *JavaScript & jQuery: Interative front-end development.* Indianapolis, IN: Wiley

**Order of execution** - the order in which statements are processed. JS processes one line of code at a time. When a statmenet needs data from another function, it stacks the new function on top of the current task.

### Execution Contexts

* Global context - code tha is in the script but not in a function.
  
  * Global scope of a variable - if a variable is declared outside of a function, it can be used anywhere.

* Function context - code that is being run within a function. Each funtion has its own function context.
  
  * Funtion-level scope - when a variable is declared within a function, it can only be used within that function.

### Execution context & hoisting

1. Prepare

- the new scope is created.

- Variables, functions, and arguments are created.

2. Execute 
  
* Now it can assign values to variables

* Reference functions and run their code

* Execute statments


### Error objects

Error objects can help find where mistakes are.

Properties:

* name - Type of error

* message - Description

* fileNumber - Name of the Javascript file

* lineNumber - Line number error


#### Built-in error objects:

* Error

* SyntaxError

* ReferenceError

* TypeError

* RangeError

* URIError

* EvalError

### Dealing with errors

1. Debug the script to fix errors

2. Handle errors gracefully - using "try, catch, throw, and finally statements.

### Debigging Workflow

1. Look at error message

2. Cosole log to see how far code is running

3. Breakpoints.



-----

[**<== BACK**](201-toc.md)
