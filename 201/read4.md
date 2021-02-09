# HTML Links, JS Functions, and Intro to CSS Layout
## HTMLLinks
#### _links_ are created using the `<a>` tag the adding the location link inside it using the `herf = ""` attribute

![ex](https://i.ibb.co/g6NfXdt/1.jpg)

#### _links_ are used to link:

| between | URL |
| ------- | --- |
| website to another | absolute URL `https://www.google.com/` |
| page to another (same website) | relative URL `about-us.html` |
| part to part (same page) | `#partId` |
| open a new window | `https://www.google.com  target = "blank"` |
| email links | `mailto:name@gmail.com` |

## JS Functions
#### A function is a list of statements (instructions) performs a specific task. It is a way to perform the same task in different parts in the code file without retyping the statements. It is a useful technique to make a fast executed programmed file because functions are not executed until they are called. In JavaScript there is a lot of saved functions can be used to modify the HTML content or make them interactive with the user as `document.write();`. functions are called by their names and filling their parameters with either values or variables contain values if function parameters are existed.Functions are made up by two methods:

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

## Intro to CSS Layout
#### layout for HTML elemnts can be displayed in two ways:
  - **block level**
  - **inline**
#### for block level elements it starts in new lines while the inline elements can flow between surronding texts.
#### controlling the elements position can be done by:
  1. **normal flow**
  2. **relative positioning**
  3. **absolute positioning**
  4. **fixed positioning**
  5. **floating elements**
