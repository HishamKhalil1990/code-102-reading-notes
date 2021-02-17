# Error Handling & Debugging
### Errors are happened due code writing mistakes. To find the error source, `console` tool is a good item that built up in the browser to track and showing errors. However, in order to find the error source, it is useful to understand: 
  - **code execution order** 
  - **the variables and functions execution contexts (scope)**
### When a function needs data from another function that. The interpreter stacks the new function above the current function. This is because interpreter run one line of the code at a time. When interpreter enters a new execution context, it has to do two activities which are:
  1. **_Prepare_ the context by creating scope, variables, functions and this value are determined**
  2. **_Execute_ functions, statements and a assign the variables values**
### Each execution context has its own scope for variables and functions, however it can access its parents scope and not the opposite. This is known as a **_lexical scope_**
### When errors occur in JavaScript. The interpreter stops, throws an exception and looks for **_exception-handling_** code. To find the error, error objects using browser tools can help. Some of the error objects are:

![ex](https://i.ibb.co/7NtHqC3/1.jpg)

### To deal with these objects then one of the two methods can be used:
#### 1. Debug the scrip using the browser console to fix errors by:
  - **knowing where the problem is**
  - **knowing what the problem is**
#### some of the useful tools in debugging are:
  - **breakpoints which allow the programmer to pause the execution at a point and know what are the variables current values**
  - **stepping through code which allows the programmer to run the code step by step between breakpoints back and forth**
  - **conditional breakpoints which allow to trigger a breakpoint if a specified condition is met**
#### breakpoints are done using the word `debugger` in the code
#### 2. Handle errors gracefully by:
  - **`try` to execute a code statements**
  - **`catch(exception)` to execute another code statements only if try throws an error**
  - **`finally` to execute a code statements always after the previous steps wither they succeed or not**

    ![ex](https://i.ibb.co/ZKz7Jt9/2.jpg)

#### Errors can be thrown before the interpreter creates them by using `throw new Error(‘message’);` which creates an error object. Some of common errors are:
  - **_a case sensitive error_**
  - **_missed/extra character_**
  - **_data type issues_**
