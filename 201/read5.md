# Images, Color and Text
## Images
#### They can be added in HTML using `<img>` tag. By adding values to the tag attributes, images are showed and described in web page. The attributes are:

| attribute | description |
| --------- | ----------- |
| `src=” ”` | add the image source |
| `alt=” ”` | add description for the image if it doesn’t appear |
| `title=” ”` | add information to images |
| `height` | add height to images |
| `width` | add width to images |

#### images can be described as inline elements, their position is managed using `align` attribute. It allows texts to flow right or left to the image. To add images then

  - **save the in the right format as `jpg` and `gif`**
  - **save them in the right size as `100*200 px`**
  - **use the correct resolution as `72 ppi`**

#### images usually come with captions. Images from share same caption can be put inside a `<figure>` and their description is put in `<figcaption>`

## Colors
#### methods to specifying colors for background and foreground and fonts in CSS:
| method | description | example |
| ------ | ----------- | ------- |
| RGB values | `color:rgb(red,green,blue);` | `color:rgb(100,100,90);` |
| RGBA values | `color:rgb(red,green,blue,opacity);` | `color:rgb(100,100,90,1);` |
| HSL values | `color:rgb(hue,saturation,lightness);` | `color:hsl(0,50%,78%);` |
| HSLA values | `color:rgb(hue,saturation,lightness,alpha);` | `color:hsl(0,50%,78%,1);` |
| HEX code | Hexadecimal code | `color:#ee3e80;` |
| color name | its name | `color:DarkCyan;` |

### when picking colors for background and foreground, it’s important to ensure that there is enough contrast for the text to be legible

## Texts
#### text fonts typeface is divided into categories:

  - **serif**
  - **sans – serif**
  - **monospace**
  - **cursive**
  - **fantasy** 

#### for fonts, there are some properties can be styled using `CSS` as weight, style and stretch. however, specifying the typeface is done in `CSS` by `font-family` like `body {font-family : Georgia , times , serif;}`. For the font size, it’s changed by `font-size` like `body {font-size : 10px}` or `body {font-size : 120%}` or `body {font-size : 1.3em}`. Sometimes the font type is not provided by the user computer, using `@font-face` allows the user to download it using the URL source like `@font-face { font-family : ’ChunkFiveRegular’; src : url(‘fonts/chunkfive.eot’); }`. Some of the texts styling are:

| attribute | description |
| --------- | ----------- |
| `text-transform` | transform letters `uppercase`, `lowercase` and `capitalize` |
| `text-decoration` | make texts `underline`, `overline` and `blink` |
| `latter-spacing` | make spaces between letters |
| `word-spacing` | make spaces between words |
| `text-align` | move the texts `left`, `right`, `center` and `justify` | 
