# Transforms, Transition and Animations
## Transforms:
#### A transform is an element layout attribute. It is used to position the element in different angles. Transform property includes multiple vendor prefixes to adapt with different browser as:
 - **`-webkit-transform: scale(1.5);`**
 - **`-moz-transform: scale(1.5);`**
 - **`-o-transform: scale(1.5);`**
 - **`transform: scale(1.5);`**
#### Transform is came with two different settings which are:
 1. **two-dimensional and it includes:**

    | property | function | script |
    | -------- | -------- | ------ |
    | 2D rotate | rotate the element | `transform: rotate(20deg);` |
    | 2D scale | change the appeared size for the element | `transform: scale(.75);` |
    | 2D translate | push and pull an element in different directions | `transform: translate(-10px, 25%);` |
    | 2D skew | distort elements on the x-axis, y-axis, or both | `transform: skew(5deg, -20deg);` |

    - **Combining transform values is allowed as in `transform: skew(10deg, 20deg) translateX(20px);`**
    - **The origin points for the element can be transformed as in `transform-origin: top left;`**
    - **3D perspective view can be done for the 2D element using `transform: perspective(200px) rotateX(45deg);`** 

2. **three-dimensional and it includes:**

    | property | function | script |
    | -------- | -------- | ------ |
    | 3D rotate | rotate the element | `transform: perspective(200px) rotateZ(45deg);` |
    | 3D scale | change the appeared size for the element | `transform: perspective(200px) scaleZ(.25) rotateX(45deg);` |
    | 3D translate | push and pull an element in different directions | `transform: perspective(200px) translateZ(50px);` |

    - **For a 3D skew, 2D elements are skewed on x/y-axis to transformed three-dimensionally**

#### Transform style is placed in the **parent element** . using `transform-style: preserve-3d;` value allows the transformed children elements appearing in three-dimensional plane while the `transform-style: flat;` value forces the transformed children elements appearing in two-dimensional plane.

## Transition
#### Transition is when pseudo-classes as `:hover` , `:focus` , `:active` , and `:target` are used to change the element style through the element states. Transition has four properties attributes which are:
 1. **`transition-property` it used to determine the element property to be changed as the `background-color`**
 2. **`transition-duration` determine the time needed to change the property as `1s`** 
 3. **`transition-timing-function` determine the changing speed**
 4. **`transition-delay` determines how long a transition should be stalled before executing**

## Animations
#### Animation is used to control the element visual interactions from one state to another more than the transition. For using animation, the key frames rule `@keyframes` must be use before the animation property declaration as in:

![ex](https://i.ibb.co/7CnyGw3/2.jpg)

#### Once the property is declared then:
  - **`animation-name` is used to assign the property for the element.**
  - **`animation-duration` determine the time needed for doing the animation**
  - **`animation-timing-function` determine the animation speed**
  - **`animation-delay` determines how long it should takes before starting the animation**
  - **`animation-iteration-count` determine how many times to repeat the animation**
  - **`animation-direction` determine the animation execution direction**
  - **`animation-play-state` determine the animation current state**
  - **`animation-fill-mode` keep the styles declared within the last specified keyframe**

![ex](https://i.ibb.co/L5D6WT6/3.jpg)

[What Google Learned From Its Quest to Build the Perfect Team](../201/read15.md)