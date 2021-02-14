# Object-Oriented Programming, HTML Tables
## Object-Oriented Programming
#### to create an object, there are two ways:

| method | script | result |
| ------ | ------ | ------ |
| the word new and the object constructor | `var objectName = new object();` | create a blank object |
| literal notation | `var objectName = {property : value, method : function (){statements;}};` | create an object |

#### Properties and methods can be added, updated, accessed and deleted by:

| function | script |
| -------- | ------ |
| add | `objectName.newProprty = “value”;` / `objectName.newMethod = function () {statements;};` |
| update property | `objectName.proprty = “new value”;`
| access | `objectName.proprty;` / `objectName.method();` |
| delete | `delete objectName.proprty;` / `delete objectName. method();` |

#### To create instances from the same object then:

![ex](https://i.ibb.co/ZBDrfJX/1.jpg) 

#### When using objects variables in methods statements, the word `this` must be used to specify the property location if the object name isn’t used inside the object as in `console.log(this.propertyName);`
#### Arrays are a special type of object. However both can be stored in each other.
#### There are three groups of built-in objects:
 1. **document object model** [ex](https://i.ibb.co/D47ZZXD/dom2.jpg)
    - ![ex](https://i.ibb.co/j6SryBQ/dom.jpg)   
 2. **browser object model** [ex](https://i.ibb.co/GQD70w1/bom2.jpg)
    - ![ex](https://i.ibb.co/82LkvrV/bom.jpg)
 3. **global JavaScript objects** [ex](https://i.ibb.co/P6pS55T/gjo-math.jpg)
    - ![ex](https://i.ibb.co/kDX2Bn7/gjo.jpg)

## HTML Tables
#### Tables are type of displaying information in grid format. The structure for a table in HTML is:

| element | function |
| ------- | -------- |
| `<table>` | define a table element |
| `<tr>` | define a new row in the table |
| `<td>` | define a cell in the row |
| `<th>` | define a heading for either columns or rows |

#### For long tables:

| element | function |
| ------- | -------- |
| `<thead>` | define the table heading |
| `<tbody>` | define the table body |
| `<tfooter>` | define the table footer |

#### To span cells laterally, the attribute `colspan = “no. of columns”` is used and to span cells vertically, the attribute `rowspan = “no. of rows”` is used. To define width dimension for a cell, attribute `width = “width size”` is used. Background color for table and cells are changed by `bgcolor = “color”` and border for the table is done by `border = “number for border size”`
