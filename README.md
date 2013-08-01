carousel
========

A awesome mini carousel plugin using CSS3

A CSS3 Cycling Slideshow! Thanks to CSS3, we can create effects and animations without using JavaScript, which will facilitate the work of many designers.

## Examples

[http://stupig.me/lab/carousel](http://stupig.me/lab/carousel)

## Usage
use like this: 
```javascript
    $.carousel(elment, {
        width: 320,
        height: 50,
        items: [
            {
                url: '/img0.png'
            },
            {
                url: '/img1.png'
            },
            {
                url: '/img2.png'
            },
            {
                url: '/img3.png'
            },
            {
                url: '/img4.png'
            }
        ]
    });
```
or:
```javascript
    $elem.carousel({
        width: 320,
        height: 50,
        items: [
            {
                url: '/img0.png'
            },
            {
                url: '/img1.png'
            },
            {
                url: '/img2.png'
            },
            {
                url: '/img3.png'
            },
            {
                url: '/img4.png'
            }
        ]
    });
```
Or you can use custom snippet:
```javascript
    $elem.carousel({
        width: 320,
        height: 50,
        snippet: '\
            <li class="animation0">\
                <img src="/apple.png" />\
            </li>\
            <li class="animation1">\
                <img src="/egg.png" />\
            </li>\
            <li class="animation2">\
                <img src="/ball.png" />\
            </li>\
        '
    });
```

## Properties

### width:
*Number* The width of the carousel container.

*default* 680

### height:
*Number* The height of the carousel container.

*default* 320

### itemShowTime:
*Number* Set every item's showing time span, unit is second

*default* 3

### itemTransferTime:
*Number* Set every item's transfer time span, unit is second

*default* 2

### direction
*String* Select the sliding direction, "horizontal" or "vertical"

*default* 'horizontal'

### transfer
*String* Select the transfer mode, "fade" or "slide"

*default* 'fade'

### effect
*String* Select the slide effect mode, "linear" "ease" "ease-in" "ease-out" or "ease-in-out"

*default* 'linear'

### snippet
*String* Set carousel item's HTML source code, optional.

*default* ''

### item
*Collection* Set carousel items data, optional. if u already set snippet, this option will be useless

*default* []

### progressBar
*Boolean || Object* Set whether to display progressBar. If true, set its style

*default* `{ height: 5, effect: 'ease-out', background: '#000' }`

*hint* 

height: *Number* Set the height of the progress bar
effect: *String* set the effect of the progress bar
background: *String* set the background of the progress bar

### indexes
*Boolean || Object* Set whether to display indexes. If true, set its style

*default* `{ height: 12, activeBackground: '#00a3ce', normalBackground: '#ccc' }`

*hint*

height: *Number* Set the height of the index bar
activeBackground: *String* Set the background of the active item
normalBackground: *String* Set the background of the normal item
