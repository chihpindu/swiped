# Swiper.js
[![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://raw.githubusercontent.com/mishk0/swiper/master/LICENSE)

[Demo](http://mishk0.github.io/swiper/) (use mobile or emulate touches mode on your browser)

## API

### Swiper(options)

- `options` (object) - Options to configure a new instance of Swiper.
- `[options.duration]` (number) - The time (milliseconds) to open/close the element. Default: `200`.
- `[options.tolerance]` (number) - Default: `150`.
- `[options.time]` (number) - Time for short swipe. Default: `200`.
- `[options.left]` (number) - Distance for swipe from left to right. Default: `0`.
- `[options.right]` (number) - Distance for swipe from right to left. Default: `0`.
- `[options.list]` (boolean) - Elements depend on each other. Default: `false`.


```js
var swiper = Swiper.init(options);

swiper.open();
swiper.close();
swiper.toggle();
```

## Usage

Example of the html markup for single element:
```html
<div class="foo">
    elem1
</div>
```
for multiple:
```html
<ul class="bar">
    <li>
        elem3
    </li>
    <li>
        elem4
    </li>
    <li>
        elem5
    </li>
</ul>
```

initialization for single element:
```js
var s1 = Swiper.init({
    query: '.foo',
    right: 300
});
```
for multiple:
```js
var s3 = Swiper.init({
    query: '.bar li',
    list: true,
    left: 200,
    right: 200
});
```
