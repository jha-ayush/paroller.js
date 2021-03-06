# paroller.js

[![npm](https://img.shields.io/npm/v/paroller.js.svg)](https://www.npmjs.com/package/paroller.js)

A lightweight jQuery plugin that enables parallax scrolling effect.
  - You can use it on elements with background property or on any other element
  - While scrolling elements can move: vertical, horizontal
  - Manipulated through *html data-** attributes
  - Mobile ready
  - Easy to use

**DEMO:** [example page](https://tgomilar.github.io/paroller.js/)

## Install
Before closing ```</body>``` element include:

1. [jQuery](http://jquery.com/download/)
2. [jquery.paroller.js](https://github.com/tgomilar/paroller.js/tree/master/dist)


#### npm
```sh
$ npm install paroller.js
```
#### Bower
```sh
$ bower install paroller.js
```
#### Yarn
```sh
$ yarn add paroller.js
```
#### Run
```javascript
// initialize paroller.js
$("body").paroller();
```
```html
<!-- select element -->
<div data-paroller-factor="0.3"></div>
```

## Usage
### data attribute
To enable Paroller on element you have to add *data-paroller-factor* to selected element. 
*data-paroller-factor* sets speed and distance of element's parallax effect on scroll. 


| data-* | value | default value |
| ------ | ------ | ------ |
| data-paroller-factor | invokes *jquery.paroller.js* functionality. It sets elements offset and speed. It can be positive (0.3) or negative (-0.3). Less means slower. | 0 |
| data-paroller-type | background, foreground | background |
| data-paroller-direction | vertical, horizontal | vertical |

### JavaScript
```javascript
// initialize paroller.js
$(window).paroller();
```
```javascript
// initialize paroller.js and set attributes for #element
$("#element").paroller({ factor: '0.5', type: 'foreground', direction: 'horizontal' });
```

### Todos

 - direction: diagonal

License
----

MIT

