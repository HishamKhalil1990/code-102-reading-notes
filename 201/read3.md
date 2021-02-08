# HTML Lists, Control Flow with JS, and the CSS Box Model
## HTML Lists
#### In HTML there is two types of lists to define items list:
  - **unordered lists `<ul>`**
  - **ordered lists `<ol>`**
### ordered lists are numbered while the unordered aren’t. To define items in the list for both, a list tag `<li>` is used inside them for each item.
### there is another type of lists called the definition list `<dl>` which is used to show a list of terms to be define <dt> and their definitions `<dd>`. Tags `<dt>` and <dd> are put – as many as needed –  inside the `<dl>` tag.
#### lists can be nested in each other

![ex](https://i.ibb.co/zPfFWsz/3.jpg)

## CSS Box Model
#### boxes are used to make limited spaces and show the insider contents in them without spreading the contents all over the page. A box is made by the contents tag properties in CSS file. Some of the important properties to create a box are:

| property | description |
| -------- | ----------- |
| height | define the box height |
| width | define the box width |
| overflow | define the scroll property |
| border | define a the box limits border lines | 
| margin | define spacing between the box and the outside contents |
| padding | define spacing between the box and the inside contents | 

![ex](https://i.ibb.co/dKXD5gv/9.jpg)

## Control Flow with JS
#### one of the conditions flow control is a `switch` statements. It compares the `switch value` with `cases values`. Once the values are identical, `to do statements` are run, else it jumps to the next case until it reach the `default` value which similar to the `else` block in the `if` statement

`switch (switch value) {`
        `case  ‘value1’`
              `to do statements`
              `break!`      
        `case  ‘value2’`
              `to do statements`
              `break!`                  
        `case  ‘value3’`
              `to do statements`
              `break!`                  
         `default`
              `to do statements`
              `break!`       
`}`                       

#### Loops are codes repeat running their inside instructions (statements) as long as the loop condition is true. Loops are consist of:

  1. **_initialization_ is the initial value for the condition variable**
  2. **_condition_ is the condition variable compared with a limit**
  3. **_update_ is the new updated value for the condition variable**

#### Some of these loop scripts are:
  - **while loop**

`var counter = 1;`
`while (condition) {`
      `to do statements` 
      `counter ++`
`}`

  - **for loop**

`var counter;`
`for (counter = 1 , condition , counter ++) {`
      `to do statements` 
`}`
