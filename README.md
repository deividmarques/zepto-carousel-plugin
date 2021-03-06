# Zepto Carousel Plugin (Webkit only & Experimental)

A lightweight zepto plugin totally based on [SwipeView](https://github.com/cubiq/SwipeView). Live demo is [here](http://etanxing.github.com/).

#### html
``` html
<div class="container">
</div>
<div class="slides">
    <div class="slide">Page1</div>
    <div class="slide">Page2</div>
    <div class="slide">Page3</div>
    <div class="slide">Page4</div>
</div>
```
#### javascript
``` javascript
$('.container').carousel({slides: $('.slides').children()});
```

#### events
``` events
$('.container').on('swipeview-flip', function(e, masterPages, options, currentMasterPage) {
	....
}

$('.container').on('swipeview-moveout', function(e, masterPages, options, currentMasterPage) {
	....
}

$('.container').on('swipeview-movein', function(e, masterPages, options, currentMasterPage) {
	....
}

$('.container').on('swipeview-touchstart', function(e, masterPages, options, currentMasterPage) {
	....
}
```