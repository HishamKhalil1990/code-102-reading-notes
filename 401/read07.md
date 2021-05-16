# Python Scope
## Scope
#### Scope can be defined as the area where a variable, function or object can be accessed.  It determines the visibility of a variable, function and object within the code. the scope for these depends on where they are decleared in the code
#### In Python scope concept is presented using the Local, Enclosing, Global and Built-in (LEGB) rule.
#### Some of scope advantges is writing more reliable and maintainable programs because helps to avoid or minimize bugs related to name collision in the programs.
#### In Python, variables come into existence when they are assigned by a value. functions and classes exist after they are defined using def or class, respectively and modules exist after they are imported so where variables are assigned or function or class is defined the code determines the scope or visibility of them
## Local scope
#### Local scope is the body of any Python function or lambda expression. it variables contains the names that are defined inside the function. they are visible in the function. the scope is created at function call, not at function definition
## Enclosing (Nonlocal) scope
#### Nonlocal scope only exists for nested functions. so If the local scope is an inner or nested function, then the enclosing scope is the outer or enclosing function scope.The variables names in the enclosing scope are visible in the inner and enclosing functions.
## Global scope
#### Global scope is the top-most scope in a Python program. it contains all of the variables names that are defined at the top level of a program. they are visible from everywhere in your code.
## Built-in scope
#### Built-in scope is a special Python scope. it is created or loaded whenever a script is run or opened. This scope contains variables names such as keywords, functions, exceptions, and other attributes that are built into Python and they are also available from everywhere in the code.
## Modifying the scope Behavior 
#### Python provides two keywords that allow modifying the variables names scope and they are:
- `global` which used to assign directly a new value to a variable which was defined outside a function
- `nonlocal` which used to assign a new value to a variable in the inner scope where the variable was defined in the outer scope inside a function