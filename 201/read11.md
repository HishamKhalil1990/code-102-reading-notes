# Audio, Video and Images
## Audio and video
#### To embed an audio and a video in HTML, `<audio>` and `<video>` tags are used. Inside the media tags, the media source tag with the source and the type is placed as `<source src=’source..mp4’ type=’video/mp4’>` . To play the media programmatically, the `HTMLMediaElement.play();` and for pausing `HTMLMediaElement.pause();` . To assign buttons for media playing then `<button class="play" data-icon="P" aria-label="play pause toggle"></button>` and media pausing then ` <button class="stop" data-icon="S" aria-label="stop"></button>` . The buttons layout is controlled in CSS as:
  - **`visibility: hidden;`**
  - **`opacity: 0.5;`**
  - **`width: 400px;`**
  - **`border-radius: 10px;`**
  - **`position: absolute;`**
  - **`bottom: 20px;`**
  - **`left: 50%;`**
  - **`margin-left: -200px;`**
  - **`background-color: black;`**
  - **`box-shadow: 3px 3px 5px black;`**
  - **`transition: 1s all;`**
  - **`display: flex;`** 
#### To add functionally to buttons using JavaScript then:
  1. **Create a JavaScript file called `custem-player.js`**
  2. **Get the elements id and store it in variables as follows:**
    ![ex](https://i.ibb.co/DDtwxtB/3.jpg)

  3. **Remove the default browser controls from the video, and make the custom controls visible using:**
        - ` media.removeAttribute('controls');`
        -  `controls.style.visibility = 'visible';`
  4. **Add an event listener for play variable as `play.addEventListener('click', playPauseMedia);`**
  5. **For the `function playPauseMedia` then:**
    ![ex](https://i.ibb.co/m0CgJ9s/4.jpg)

  6. **Add an event listener for stop and media variable as `stop.addEventListener('click', stopMedia);` and `media.addEventListener('ended', stopMedia);`**
  7. **For the function `stopMedia` then:**
        ![ex](https://i.ibb.co/MRHpwJz/5.jpg)
  

## Images
#### Html support adding images using `<img>` tag. The element size can be controlled using CSS by `height` and `width` attributes were the values can be a pixel number as `100px` or a percentage as `50%` . The element alignment can be controlled be the `float` attribute where the image can be floated to `right` or `left`. However, to center an image the attribute `display` is used with a value of `block` and a `margin: 0px auto;` . Images can be assigned as background image for a container element by using `background-image: url(‘image-relative/abslute-path’);` . The background image can be sized in the container element by `background-size` and the values can be a number as `100px 400px` or a percentage as `50% 70%` for height and width. When an image is assigned as a background image, if the width or height is less than the container width or height then the image will be repeated to fill the empty space. The repeat is controlled by `background-repeat` where the values can be:
![ex](https://i.ibb.co/pxC3MRM/2.jpg)
  - **`no-repeat` for height and width**
  - **`repeat-x` the image will be repeated horizontally**
  - **`repeat-y` the image will be repeated vertically**
#### Background images can be made as scrolled up and down images and its position is controlled by `background-position` where the position can be:
#### Background images contrast can be one of three:
  1. **High contrast**
  2. **Low contrast**
  3. **screen**
