# Functions
## Introduction:
### A function is a list of statements (instructions) performs a specific task. It is a way to perform the same task in different parts in the code file without retyping the statements. It is a useful technique to make a fast executed programmed file because functions are not executed until they are called. In JavaScript there is a lot of saved functions can be used to modify the HTML content or make them interactive with the user as `document.write();`. functions are called by their names and filling their parameters with either values or variables contain values if function parameters are existed. 

## Function construction
### Functions are made up by two methods:

| method | script |
| ------ | -------- |
| function declaration  | `function calculate(length,width) {area = length*width; return area;}` |
| expression function  | `var calculate = function(length,width) {area = length*width; return area;}` |

### where are:
  1. **`function` is the function keyword**
  2. **`calculate` is the function name**
  3. **`(length,width)` are the function parameter could be more, less or null if function doesn’t need**
  4. **`area = length*width` is a function statement to do a task, could be more than one**
  5. **`return area` is the function returning value after the run and its optional depending on the function task**

### the previous function is called by `calculate(x,y);` where x and y are the function arguments, they are variables contain a number values assigned by the function user. Note the user can assign values directly as a function arguments `calculate(5,10);` but a best practice to assign variables.

**go back to** [home page](README.md)

