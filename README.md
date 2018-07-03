# [GISC Image Slider]

> - Latest Version v2.0.0
 
[GISC Image Slider] is most beautiful and easy to use image slider with unique visual effects. 

GISC Image Slider is a click-to-enlarge-and-view-slider wizard to create awesome image slider
without extra coding. 
  
Responsive, and fully accessible as made up of a pure CSS. Supported by all browsers, all devices etc. 

### Getting started

Using GISC Image Slider is straightforward. First, you need to include gisc.min.js and gisc.min.css in your web site :

CSS File :

```HTML
<link rel="stylesheet" href="gisc.min.css">
```

Javascript File :

```HTML
<script type="text/javascript" src="gisc.min.js"></script>
```

#### Usage

e.g. Suppose, you want to show Image Slider on click of an image thumbnail, then you want to provide list of all images (you want to show in slider) in `ul` tag. Please write `ul` tag immediately below the image / input (button) / button on click of which, you want to show Image Slider. Please refer sample code below or you can see `example.html` :

```HTML
<img src="http://www.example.com/image.png" />
<ul class="image-list g-keep-hidden">
  <li>http://www.example.com/image1.png</li>
  <li>http://www.example.com/image2.png</li>
  <li>http://www.example.com/image3.png</li>
</ul>
```

In above example, Image Slider enables when you click to Image `http://www.example.com/image.png`.

NOTE : Please add `g-keep-hidden` class to `ul` tag. It will avoid showing ul tag at the time of DOM load.

Initialize with `GImageSlider` method :

```javascript
$('.image-list').GImageSlider();
```

#### Options

You may set GImageSlider Options with `$('.image-list').GImageSlider(options)`.

##### 1. imageCount
* Type : `Boolean`
* Default : `false`

If `true`, `imageCount` shows current image number out of total image count, at the top left corner of the image.
e.g. `1/10`

##### imageTitle
* Type : `Boolean`
* Default : `false`

If true, `imageTitle` shows current image description at the bottom of the image.
  - NOTE : You need to provide title attribute for `<li>` tags for which you want to show image description.
  - e.g. `<li title="This is dummy Image Description">http://www.example.com/image1.png</li>`

##### animation
* Type : `String`
* Default : `fade`

You can use `animation` to change images transitions.
  - Supported Transitions : `fade` `slide`
  
##### enableLog
* Type : `Boolean`
* Default : `false`

In Case of any issue, you can set `enableLog` to `true` and debug it from browser console.

### NOTE :

1. Requires jQuery (greater than v2.0)
2. You can use jQuery Mobile to use Swipe left, Swipe right on various devices.

### Browser support

* Mozilla Firefox
* Google Chrome
* Internet Explorer
* Safari
* Opera

## Author

Ghanashyam Chaudhari (mr.ghchaudhari@gmail.com)