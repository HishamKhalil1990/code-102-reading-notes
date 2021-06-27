# React
## Introducing JSX
### JSX is a syntax extension to JavaScript. it is similar to template language, but it comes with the full power of JavaScript. JSX produces React `elements`
### Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both. We will come back to components in a further section, but if you’re not yet comfortable putting markup in JS, this talk might convince you otherwise
### After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.
### React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered. This helps prevent XSS (cross-site-scripting) attacks
## Rendering Elements
### Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements. Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like
### React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.
## Components and Props
### Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. they are like JavaScript functions. They accept arbitrary inputs called `props` and return React elements describing what should appear on the screen
### When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object `props` .
### Components can refer to other components in their output. This lets us use the same component abstraction for any level of detail. A button, a form, a dialog, a screen: in React apps, all those are commonly expressed as components. Typically, new React apps have a single App component at the very top
### Whether you declare a component as a function or a class, it must never modify its own props. All React components must act like pure functions with respect to their props.
## State and Lifecycle
### You can convert a function component to a class in five steps:
- Create an `ES6 class`, with the same name, that extends `React.Component`.
- Add a single empty method to it called `render()`.
- Move the body of the function into the `render()` method.
- Replace `props` with `this.props` in the `render()` body.
- Delete the remaining empty function declaration.
### In applications with many components, it’s very important to free up resources taken by the components when they are destroyed.
### There are three things you should know about `setState()` which are:
1. Do Not Modify State Directly
2. State Updates May Be Asynchronous
3. State Updates are Merged
## Handling Events
### Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:
* React events are named using camelCase, rather than lowercase.
* With JSX you pass a function as the event handler, rather than a string.
### React defines these synthetic events according to the W3C spec, so you don’t need to worry about cross-browser compatibility. React events do not work exactly the same as native events. When using React, you generally don’t need to call addEventListener to add listeners to a DOM element after it is created. Instead, just provide a listener when the element is initially rendered.
### When you define a component using an ES6 class, a common pattern is for an event handler to be a method on the class. 
### Inside a loop, it is common to want to pass an extra parameter to an event `e` handler like `id`. the `e` argument representing the React event will be passed as a second argument after the `id`. With an arrow function, we have to pass it explicitly, but with bind any further arguments are automatically forwarded