# THE CALL STACK and debugging
## call stack
### call stack is how interpreter tracking the functions and add them to the stack then run where their calls are reached. any function is finished is no longer on the stack.
### on of the reasons that call stack is important is the concept of **Asynchronous programming** which means the code is run one by one. so functions are waiting in the stack until their turn reached.
### it should mentioned the call stack cycle is **last in - first out** .
## debugging
### debugging is how to find the error place, the type of the error, the cause of the error and then fix it.
### for error types, these are some examples:
- Syntax errors
- Range errors
- Type errors
- Reference errors
### the debugging process is done by using either `console.log()` or `debugger` and for handling the error, `catch()` is used. 