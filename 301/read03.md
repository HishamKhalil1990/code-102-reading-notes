# MUSTACHE and FLEXBOX
## MUSTACHE
#### Mustache is a logic-less template syntax works by expanding tags in a template using values provided in a hash or object. Javascript templating is technique used for showing the client-side view templates with Javascript by using a JSON data source. mustache.js is an implementation of the mustache template system in JavaScript. It is considered as the base for JavaScript templating. 
#### so when run `Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });` When Mustache compiles syntax, it looks for the actual value of `name` property - which is `“Sherlynn”` - in the object we pass in, and replace of `{{ name }}` .
#### it can be noticed Mustache is a specification for a templating language.
#### Mustache-Express is a way to use Mustache and Express together easily as in:

![ex](https://i.ibb.co/rdBkQgF/3.jpg)


## FLEXBOX
#### FLEXBOX is a CSS method to rearrange a container element's children. it starts by choose `display:flex` in the container CSS. flexbox has different attriburtes for parent element and they are:
1. `flex-direction` which establishes the main-axis and defining the direction of the axis in the container. it has different values as:
    - `row` (default)
    - `row-reverse` right to left
    - `column` same as row but top to bottom
    - `column-reverse` same as `row-reverse` but bottom to top
2. `flex-wrap` which allows the items to wrap as needed. it has different values as:
    - `nowrap` (default)
    - `wrap` flex items will wrap onto multiple lines from top to bottom.
    - `wrap-reverse` flex items will wrap onto multiple lines from bottom to top
3. `flex-flow` which is a shorthand for `flex-direction` and `flex-wrap` properties it has different values as:
    - `row wrap` a combination of `row` and `wrap`
    - `row-reverse wrap` a combination of `row-reverse` and `wrap` 
    - `column wrap` a combination of `column wrap` and `wrap`
    - `column-reverse wrap` a combination of `column-reverse` and `wrap` 
4. `justify-content` , `align-items` and `align-content`defines the alignment along the main axis and helps distribute extra free space leftover. the differnce between `justify-content` and `align-items` or `align-content` the directions are perpendicular to each other. they have different values as:
    - `flex-start` (default)
    - `flex-end` items are packed toward the end of the flex-direction
    - `center` items are centered along the line
    - `space-between` items are evenly distributed in the line; first item is on the start line, last item on the end line
    - `space-around` items are evenly distributed in the line with equal space around them.
#### flexbox has different attriburtes for children element and they are:
1. `order` which is used to re-order the child and it's value is an intger
2. `flex-grow` which defines the ability for a flex item to grow if necessary
3. `flex-shrink` which defines the ability for a flex item to shrink if necessary
3. `align-self` which allows to re-align the child 




