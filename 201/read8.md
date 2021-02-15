# Layout in CSS
### CSS deals with HTML elements as they are existed in boxes. These boxes can be appeared as a **_block-level_** or **_inline box_** . For the block-level, it starts in a new line while the inline box can flow surrounding texts.
### controlling the elements position can be done by:

| position type | attribute | function |
| ------------- | --------- | -------- |
| normal flow | `position: static` | it’s the normal state for element position |
| relative positioning | `position: relative` | it moves the element relative to its normal position |
| absolute positioning | `position: absolute` | the surrounding elements located as the element isn’t there |
| fixed positioning | `position : fixed` | it fixes the element in its place | 
| floating elements | `float : right` | it allows the element to flow to the far right/left and the other elements flow around it |

### For the fixed position, next elements can appear on the top of the fixed element using the overlap property by using `z-index: 5` for example.
### when float is done for an element, the next elements will be affected. To stop the influence for floating element to the next elements, `clear` attribute is used in CSS as in the following:
  - **`clear: lfet`**
  - **`clear: right`**
  - **`clear: both`**
  - **`clear : none`**
### For a web page, its layout should be appropriate for different screen sizes. Screen resolution is number of dots per inch. It must be noted the higher the resolution the smaller the text appears. Web developers try to create pages of around 960 – 1000 pixels wide. There are two types of layout:

  1. **_fixed width layout_** : the web page layout width doesn’t change as the user screen size change
  2. **_liquid layout_** : the web page layout width will be adapted to the user screen size

### Web page designers are often use a grid layout structure to position items in the pages. It is done using CSS frameworks. For styling the page, multiple style sheets can be used like using a style sheet for some properties as layout and another style sheet for other properties as font-style control. 
