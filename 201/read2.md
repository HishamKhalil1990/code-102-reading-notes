# HTML Text, CSS Introduction and Basic JavaScript Instructions
## HTML texts
#### 1. Headings in HTML have six level `<h1- h6>` . Each next level ex: `<h3>` is a subheading to the previous one ex: `<h2>`  
#### 2. Paragraphs are surrounded by <p> tag and their texts can be marked up in two ways:
  - **_structural markup_ which are elements used to affect the structure of headings and paragraphs as the following:**

| element | script | example |
| ------- | ------ | ------- |  
| bold `<b>` | `<p> what is surrounded by the b tag appears <b> bold </b> only </p>` | [bold](https://i.ibb.co/jMGZghY/1.jpg) |
| italic `<i>` | `<p> what is surrounded by the i tag appears <i> italic </i> only </p>` | [italic](https://i.ibb.co/WkSWxbn/2.jpg) |
| superscript `<sup>` | `<p> what is surrounded by sup tag appears superscript on 4 <sup> th </sup> only </p>` | [superscript](https://i.ibb.co/5j7GKfZ/3.jpg) | 
| subscript `<sub>` | `<p> what is surrounded by sub tag appears subscript under O <sub> 2</sub> only </p>` | [subscript](https://i.ibb.co/ckhM9v9/4.jpg) |
| line break `<br/>` | `<p>  what is after the br tag appears <br/> in new line </p>` | [line break](https://i.ibb.co/BnryDF1/5.jpg) |
| theme break `<hr/>` | `<p>  what is after the hr tag appears </p> <hr/> <p> in new theme </p>` | [theme break](https://i.ibb.co/XSLNpZW/6.jpg) |

  - **_semantic markup_ which are elements provide extra information without affect the structure as the following:**

| element | script | example |
| ------- | ------ | ------- |
| strong importance `<strong>` | `<p> what is inside the strong tag has <b> strong importance </b> only </p>` |[strong importance](https://i.ibb.co/nbMhX5g/7.jpg) | 
| emphasis `<em>` | `<p> what is inside the em tag can <em> change the sentence meaning </em> only </p>` | [emphasis](https://i.ibb.co/WKfg4PQ/8.jpg) |
| long quote `<blockquote>` | `<blockquote> <p>  what is surrounded by blockquote tag has longer quote </p> </blockquote> <p> more than the others </p>` | [long quote](https://i.ibb.co/PQ9rZsk/9.jpg) |
| abbreviation `<abbr>` | `<p> what is surrounded by abbr tag as<abbr title=”professor”> prof</abbr> can be titled </p>` | [abbreviation](https://i.ibb.co/9N8VG5k/10.jpg) |
| citation `<cite>` | `<p>  <cite> the citation form </cite> in what is surrounded by cite tag </p>` | [citation](https://i.ibb.co/DCNBP09/11.jpg) |
| definition `<dfn>` | `<p>  <dfn> a definition starts after </dfn> what is surrounded by dfn tag </p>` | [definition](https://i.ibb.co/pR0F1Zm/12.jpg) |
| address `<address>` | `<address> <p> what is surrounded by address tag is address </p> </address> <p>  only </p>` | [address](https://i.ibb.co/T2vbVnj/13.jpg) |
| inserted`<ins>` | `<p> <ins> inserted item </ins> is only the surrounded text by ins tag </p>` | [inserted](https://i.ibb.co/ncK8mqk/14.jpg) |
| deleted `<del>` | `<p> <del> deleted item </del> is only the surrounded text by del tag </p>` | [deleted](https://i.ibb.co/kJyfQmy/15.jpg) |
| inaccurate something `<s>` | `<p> <s> inaccurate old price </s> is surrounded by s tag </p>` | [inaccurate something](https://i.ibb.co/c6GPLsC/16.jpg) |

_________________________________________________________________________


## CSS Introduction
#### CSS rules is used to modify HTML content features as (font size, background color,…etc.) in three ways:
  1. **inline inside the tag `<h1 style =”color:red;”> name </h1>`**
  2. **internal inside style tag `<style> h1 {color:red;} </style>` inside `<head>`**
  3. **external in CSS file which is linked to HTML by the link tag `<link  rel="stylesheet" href="styles.css" >` inside the `<head>`**
#### the first two ways are done in HTML file while the third is done in a separate file
#### CSS works by associating rules to HTML elements. The rule in CSS is consists of two parts:
  - **selector indicate to the element that will be styled**
  - **declaration indicate to the type and the value of the style that will be edited**

![ex](https://i.ibb.co/gVp4XW5/css1.jpg)

#### when CSS declaration is done inside curly brackets it assigned a value for a property

![ex](https://i.ibb.co/k4KCj4g/css2.jpg)

#### types of selectors:

| type | example | script |
| ---- | ------- | ------ |
| type selector | `p, h1, ul, il, img` and `a` | `p {color:red;}` | 
| class selector | elements how have same class attribute as `class=”paragraph”` | `. paragraph {color:red;}` |
| ID selector | elements how have id attribute as `id=”mainParagraph”` |  `#mainParagraph {color:red;}` |

#### notes:
  - **_if two selectors are identical then the priority for cascading them by CSS rules is for the most_**
  - **_all elements (child)  which are inside an element (parent) inherit all the parent properties but not the opposite_**  


## Basic JavaScript Instructions
#### JavaScript is a language based on making a statement `var name = ‘hisham’;` that groups with other statements in curly brackets `{var name = ‘hisham’;  var age = 30;  var city = ‘amman’;}` to form a code block. Comments are statements too but they are not processed when the program is run. They are made to clarify what is coded. For a single line comments `// comment` and for multiple line comments `/* comments */`. In statement, a variable `var` is a temporarily store named by a name as `age` which used to store data as `30`. 
#### 1. variables:
#### To declare a variable, a specific script is written that contains:
  - _variable keyword_ **`var`**
  - _variable name_ **`age`**
#### to assign a value for  a variable, the script becomes:
  - _variable name_ **`age`**
  - _assignment operator_  **`=`**
  - _variable value_ **`30`** 
#### variables have a data types which are divided into
  - _number_ **`30`**
  - _string_ **`‘hisham’`**
  - _Boolean_ **`true`**
  - _Array_ **`[‘a’ , ‘b’ , ‘c’]`**
#### Array variables can hold more than one value from the same datatype and it is declared in two ways:
  - _first method_
    - **array literal** 

![ex](https://i.ibb.co/Fw6QtkQ/ar1.jpg)
  - _second method_
    - **array constructor**

![ex](https://i.ibb.co/nndG82M/ar2.jpg)
#### Each value in the array has an index value to call. To assign the second value in the array colors in a another variable called newVar then, `var newVar = colors[2];`. So if newVar is logged in console using `console.log(newVar);` the result will be black.
#### To change the value in the array, it is done by `colors[1] = ‘yellow’;` then the new value for index 1 in the colors array is yellow
#### 2. expressions
#### they are used to:
   - **assign a value in a variable `var name = ‘ahmad’;`**
   - **return a single value from two or more value `var area = 10*5;`**
#### 3. operators
#### they are non-alphabetic characters used to construct expressions to perform a job as in:
![ex](https://i.ibb.co/tKGvH0K/arti1.jpg)
#### 4. decision making
#### in JavaScript they are done by the if statement which consists of a condition to be evaluated and a conditional statements to be executed depending on the condition result. The general form for if statement is `if (condition) { to do statements if yes} else { to do statements if no}`. The comparison operators that can be used in the condition are:

| operator | function |
| -------- | -------- |
| `==` | do values are equal each other ?|
| `===` | do values and datatypes are equal each other ? |
| `!=` | do values are not equal each other ? |
| `!==` | do values and datatypes are equal each other ? |
| `<` | does the left value is less than the right value  |
| `<=` | does the left value is less than or equal the right value |
| `>` | does the left value is greater than the right value |
| `>=` | does the left value is greater than or equal the right value |

#### Logical operators are `&&` , `||` and `!`. They are used to connect between two conditions or more and comparing the condition results.






