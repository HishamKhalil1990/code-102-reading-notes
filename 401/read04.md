# Classes and Objects and Thinking Recursively
## Classes and Objects
#### objects are a set of variables and functions in one single entity where classes are a kind of a template to create an objects. objects are created as `object = Class()`
#### using a class, many different objects can be created and they all hold the same set of variables and functions that belongs to that class. However, each object contains its independent copies of them.
#### accessing a function in an object is like accessing a variable using notation similar.
## Thinking Recursively
#### recursive function is a function defined to do some tasks and call itself inside its code.the function will continue to call itself and repeat its behavior until some condition is met to return a result. 
#### recursive function structure is:
- base case 
- recursive case
#### for all recursive functions each recursive call has its own execution context. so to maintain its state then:
- Thread the state through each recursive call
- Keep the state in global scope
#### Recursive Data Structures in Python, any data structure is deﬁned in terms of a smaller version of itself is considered recursive.