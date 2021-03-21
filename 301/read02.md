# JQuery and Pair Programming
## Jquery
#### Jquery is a JavaScript file which gives a simple way to select elements, perform tasks and handle events comparing to DOM.

![ex](https://i.ibb.co/nckSJ9L/2.jpg)

#### When creating a selection in Jquery, it store a reference to the corresponding nodes in the DOM tree.To use Jquery it must be added in the HTML `<body>` using `<script src=”js/jquery-1.11.0.js”></script>` .
#### when selecting element using Jquery using `$()` , a Jquery object is returned as either single element like `$(‘ul’)` or multiple element like `$(‘li’)` as shown in the following :
however, in multiple element, for get information using a method as in `let content = $(‘li’).html()` it will retrieve for the first element and when updating the information using a method as `$(‘li’).html(‘updated’)` it will update all the elements.

![ex](https://i.ibb.co/3FCNWQM/3.jpg)

#### To create a Jquery object, the interpreter must do:
 1. Find the matching nodes in the DOM tree
 2. Create the Jquery object
 3. Store the nodes reference in the Jquery object

#### to run more than one method, all needed methods are listed at a time and separated by a dot notation as `$(‘li’).hide().delay(500).fadeIn(1400)` . this referred as chaining. To check the page is ready for the code then :

![ex](https://i.ibb.co/WBDbDGQ/4.jpg)

#### for a shortcut :

![ex](https://i.ibb.co/VvB313N/5.jpg)

#### a list of Jquery methods:
##### a) for getting or updating content:
  - `.html()`
  - `.text()`
  - `.remove()`
##### b) for inserting elements:
  - `.before()`
  - `.after()`
  - `.append()`
  - `.prepend()`
##### c) for creating or removing attributes:
  - `.attr()`
  - `.removeAttr()`
  - `.addClass()`
  - `.removeClass()`
##### d) for adding style:
  - `.css()`
#### for looping all the elements returned when selecting element in Jquery, `.each()` method is used. It goes through all the elements in a selection as in:

![ex](https://i.ibb.co/W3Pb5gt/6.jpg)

#### to handle events, `.on()` method is used as in `$(‘li’).on(‘click’,function(e){let eventType = e.type});` where:
 - `.on()` event handle method
 - `’click’` type of the event
 - `function(e){}` function to do when the event is triggered
#### elements can be animated using `.animate()` method as in:

![ex](https://i.ibb.co/ZKH7bmL/7.jpg)

## Pair Programming
#### Pair Programming is when two developers are working together on a project code as a driver and a navigator
#### pair programming helps in:
- increase the work efficiency
- engaging more experiance for both programmers
- knowladge exchange between the programmers
- improve social skills
- passing a pair coding test in job interviews
- fit in companies work environment