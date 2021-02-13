# Problem Domain, Objects, and the DOM
## 1) Problem Domain
#### problem domain is the scope of the problem parts needed to be solved. By defining the problem domain, programmers can decide what are the technologies are needed, the work tasks and how to code each task and assemble the whole work. Problem domain is hard to done because it’s like assembling a puzzle parts without having a big picture for the expected result. As puzzles, code with a purpose of building component are put together so that we figure out a bigger picture of the problem domain. The big issue is that many problem domains are either have blurry picture or no picture at all. However, **_coding after defining the problem domain is much easier than start coding to figure out the problem domain_** . a good tips to define a problem domain are:
  - **understand the problem better from users** 
  - **divide the domain into clarified small functional pieces and focus on them**

## 2) Objects
#### An object is a block of variables and functions are gathered to create a model of something. In objects, variables are called properties and functions are called methods. To create an object, **_literal notation_**  method is used as in the following example. 

![ex](https://i.ibb.co/T0FxLcj/2.jpg);

#### to access the object properties and methods, dot `.` notation is used between the object and its contents as in:

| spcification | example |
| ------------ | ------- |
| properties | `var hotelName = hotel.name; or hotel[‘name’];` |
| methods | `var roomsFree = hotel.checkAvailability ;` |

#### Also, to create an object then the word `new ` and the object constructor are used `var hotel = new object();` and then properties are filled and methods are created by using the name of the object and followed by the dot notation and the name of the property `hotel.name = “Seasons”;` or the function expression `hotel.checkAvailability = function(x,y){return x-y; }`. To declare an empty object then `var hotel = {}`. 

## 3) DOM
#### **DOM** is stands for Document Object Model also known as Application Programming Interface **API**. it specifies how browsers should create a model in HTML page and how JavaScript can access and update the contents for the web paged while its’s in the browser window. **note : DOM is neither part HTML nor part of JavaScript** .
#### When a web page is loaded, the browser creates a DOM tree. The tree consists of four components which are: 
 1. **document node**
 2. **element nodes**
 3. **attribute nodes**
 4. **texts nodes**

![ex](https://i.ibb.co/2M8B4pt/3.jpg);

#### To access and update the DOM tree, to steps are needed:
 1. **locate the node that represent the wanted element**
 2. **use its content as texts, attributes and child**
#### Methods which are used to find elements in DOM tree are called DOM queries such as `getElementById(‘id’);` which used to store the location of the element within the DOM tree in a variable. Queries return:

| return | Query |
| ------ | ----- |
| elements | `querySelector(‘css selector’);` |
| node lists | `getELementsByClassName(‘class’);` |

#### For selecting element from a node lists, item(); method is used.

![ex](https://i.ibb.co/9v6QJvs/4.jpg)

#### However, because node lists is an array, selecting the element can be done by using its index `elements[0];` also, the entire nodes in the list can be modified by applying statements using loops as:

![ex](https://i.ibb.co/D4jvw53/5.jpg)

#### Having an element node can used to select another elements having with the element node a relation using one of the following five properties:
  - **parent node**
  - **previous sibling**
  - **next sibling**
  - **first child**
  - **last child**
#### after that, the value of the element can be accessed by `nodeValue;`

![ex](https://i.ibb.co/WcHSGYb/6.jpg)

#### To add or remove HTML content then two ways can be followed:
- **the innerHTML property:**
  1. **get content by `var oldContent = document.getElementById(‘one’).innerHTML;`**
  2. **set content by `document.getElementById(‘one’).innerHTML = newContent;`**
- **DOM manipulation:**
  - **for adding:**
    1. **create the element by `createElement();`**
    2. **give it a content by `createTextNode();`**
    3. **add it to the DOM by `appendChild();`**
  - **for removing:**
    1. **select the element and store it in a node variable** 
    2. **find the parent and store it in a node variable**
    3. **remove the element by `removeChild();`**

##### To add text content to a web page, `document.write();` method can be used for a simple and fast adding method.
#### once the element is stored in a node, the element attributes can be accessed or modified by:

| spcification | method |
| ------------ | ------ |
| get the attribute value of element node | `thegetAttribute();` |
| check this attribute for the element node | `has Attribute();` | 
| set a new value for the element node attribute | `setAttribute();` |
| remove the element node attribute | `removeAttribute();` |

