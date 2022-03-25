# JS Image Slideshow With Text

Using JavaScript to add image slideshows onto the webpages.
The slideshow has been built by [JS Image Slideshow](https://github.com/allc/JS-Image-Slideshow) but now with the text on it !

## Demo

[JS Image Slideshow Demo](https://scott987.github.io/JS-Image-Slideshow-With-Text/demo/)

## Setup

Include the JS Image Slideshow script and the style sheet in the html:

```HTML
<link rel="stylesheet" href="css/slideshow.css">
<script src="js/slideshow.js"></script>
```

## Usage

In the application code, create a slideshow like this:

```JavaScript
var imagePaths = ['images/0.png', 'images/1.png', 'images/2.png'];
var text=['test', 'testtest', 'testtest']
var slideshowOptions = {
    interval: 3000,
    transition: 'fadeIn',
    control: false,
    background: true,
    showtext: true,
    textcontainer: document.getElementById('text'),
    text: text
};
new Slideshow(document.getElementById('slideshow-container'), imagePaths, slideshowOptions);
```

## Options
`interval`: the timeout between images, a number represent time in ms, default `5000`

`control`: if show the control buttons, `true` or `false`, default `true`

`transition`: transition effect, `null` or `'fadeIn'`, default `null`

`background`: if the image container has black background with rounded corners, `true` or `false`, default `false`

`showtext`: if show text, `true` or `false`, default `false`

`textcontainer`: where to put text, need `showtext` option

`text`: the text list to show, need `showtext` option

## Requirements

JS Image Slideshow With Text has zero dependences.

## Credits

Slideshow Credits to Harry and Rayna.
Text funtion Credits to Scott.

## License

Licensed under the [MIT](https://github.com/scott987/JS-Image-Slideshow-With-Text/blob/master/LICENSE) license.
