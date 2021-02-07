# Introductory HTML and JavaScript
## HTML
### 1. HTML is used to describe the structure of the web page. For word documents structuring, different levels of heading can be used to show the importance level. It uses elements with opening and closing tag to describe the page structures such as `<title> title name </title>`. Some elements don’t have a closing tag such as `<img src="img_girl.jpg" alt="Girl in a jacket">`. Opening tags can contain attributes to define a style `style=”color:red;”` or add a source `src="img_girl.jpg"`. a web page consists of a head and a body. Head contain the page title and CSS and JS sources while the body contains the page components and define its appearance to the user.
### 2. HTML has different versions so, to indicate the version, `<! DOCTYPE html>` is used. Comments for clarifying the code can be written inside `<! -- comments -- >`. Elements can be identify uniquely using the ID attribute `id=”elementIDname”`. A group of identical type elements can be identify using class attribute `class=”elementClassName”`. Class and id names defined in the previous attributes are used in CSS file to define the style for the content related to the identified elements only. Elements are appear in:
  - **block as in lists `<il>`**
  - **inline as in images `<img>`**
### 3. An `<iframe>` is used to add a small window contain another page like in adding a google map. The `<meta>` element exists in <head> and contain information about web page. This element is not visible to users but fulfills a number of purposes such as telling the search engines about the page, how to create it and whether or not it is a time sensitive. HTML contains escape character that are used to define symbols such as for ampersand - & - `&amp;`. 
### 4. HTML5 layout elements which are used to divide the page body into parts such as `<header>` , `<main>` , `<footer>` and `<div>`. the element name indicate for its contents which can be a group of elements like `<p>` , `<article>` , `<a>` , `<img>` and `<li>`.
### 5. website design should satisfy four criteria to be useful and easy for the users and becomes a favorite of them. So the process for building and formatting the website should satisfy:
  - [x] **the users’ needs** 
  - [x] **easiness for finding the information by the users**
  - [x] **the ability for reaching the users goals**
  - [x] **attractiveness for users**
### to approach the previous points, they should be turned to the following questions and then answered by the developer in cooperation with the expected user:
  - **_what are the user needs ?_**
  - **_Do they need the information to be general or specified ?_**
  - **_what are the visitor want to achieve?_**
  - **_what are the techniques are used for displaying the site in comfortable easy way ?_**
### answering the questions leads for a lot of data that should be arranged by its importance and context so, websites are usually consists of pages that contain contents. some of the best methods to create pages are :
  1. **site map**
  2. **wireframe** 
  3. **visual hierarchy**
### the first one is responsible for the main idea of the page, the second is responsible about the contents shown in the page and the final one is responsible about the content appearance to users.
## JavaScript
### JavaScript is a programming language. To write a script then:
  1. **_define a goal for the program_**
  2. **_design a script as a flowcharts for the program tasks_**
  3. **_code each step using the language scripts_**
### In computer programming each physical thing can be represented as an object. It can be used through instances. For each instance of the object, it has properties which has names and values. Objects are interacted with through events (a trigger). They also have methods which are a list of instructions that represent a task.
![hotel object](https://i.ibb.co/0CQbMnK/hotel.jpg)
### web browsers are built using objects.
![browser object](https://i.ibb.co/kx4Vd8J/browser.jpg)
### in HTML pages the document object used to access and change  what content users see in the web page and respond to how the interact with it
![document object](https://i.ibb.co/K9brczc/document.jpg)
### To change the HTML contents using JavaScript, the browser interprets the HTML code and applies styling to it as the following:
  1. **receive a page as HTML code**
  2. **create a model of the page and store it in the memory**
  3. **use a rendering engine to show the page on screen**
### for constructing a web page, the following are used:

| file | function |
| ---- | ------ |
|`<html>` | content layer |
| `{css}` | presentation layer |
| `javascript()` | behavior layer |

### for linking a CSS file to HTML `<link rel=”stylesheet” herf=”css/c01.css”>`, for linking a JavaScript file to HTML `<script src=”js/add-content.js”></script>` and for placing a script in the HTML, it is done be writing the method in a script tag as `<script> document.write.(“welcome”) </script>`

