# Dracula for [Highlight.js](http://highlightjs.org)

> A dark theme for [Highlight.js](http://highlightjs.org).

![Screenshot](https://draculatheme.com/assets/img/screenshots/highlightjs.png)

## Install

1. Copy `dracula.css` to your desired directory.
2. Include the theme in your html. `<link rel="stylesheet" href="dracula.css">`

## Example

```html
<!doctype html>
<html>
  <head>
    <title>highlightjs dracula theme</title>
    <link rel="stylesheet" href="dracula.css">
    <script src="http://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.4.0/highlight.min.js"></script>
    <script>hljs.initHighlightingOnLoad();</script>
    <style>html,body,pre {margin:0;padding:0} body {background-color:#282a36} pre code {font-family:Monaco;font-size:12px}</style>
  </head>

  <body>

    <pre><code class="javascript">
// Production steps of ECMA-262, Edition 5, 15.4.4.21
// Reference: http://es5.github.io/#x15.4.4.21
if (!Array.prototype.reduce) {
  Array.prototype.reduce = function(callback /*, initialValue*/) {
    'use strict';
    if (this == null) {
      throw new TypeError('Array.prototype.reduce called on null or undefined');
    }
    if (typeof callback !== 'function') {
      throw new TypeError(callback + ' is not a function');
    }
    var t = Object(this), len = t.length >>> 0, k = 0, value;
    if (arguments.length == 2) {
      value = arguments[1];
    } else {
      while (k < len && !(k in t)) {
        k++;
      }
      if (k >= len) {
        throw new TypeError('Reduce of empty array with no initial value');
      }
      value = t[k++];
    }
    for (; k < len; k++) {
      if (k in t) {
        value = callback(value, t[k], k, t);
      }
    }
    return value;
  };
}
    </code></pre>

  </body>
</html>
```

## Team

This theme is maintained by the following person(s) and a bunch of [awesome contributors](https://github.com/dracula/highlightjs/graphs/contributors).

[![Denis Ciccale](https://avatars0.githubusercontent.com/u/539546?v=3&s=70)](https://github.com/dciccale) |
--- | ---
[Denis Ciccale](https://github.com/dciccale) |

## License

[MIT License](./LICENSE)
