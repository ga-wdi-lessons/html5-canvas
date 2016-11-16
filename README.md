# Canvas

## Learning Objectives

## Framing

HTML5's `<canvas>` element is a two-dimensional space we can use to draw things.

Some use cases...

* Draw shapes, paths, images and text
* Create animations
* Create games and other interactive experiences
* 3D rendering

## A Basic Use of Canvas

Create a `canvas` folder in your sandbox directory. It should contain `index.html` and `script.js` files...

```bash
$ mkdir sandbox
$ touch index.html script.js
```

Open the folder up in atom.
* Add a `<canvas>` element to `index.html`. It canvas needs two attributes, `width` and `height`.
* Link to a jQuery CDN

```html
<!-- index.html -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Canvas</title>
</head>
<body>
  <canvas width="500" height="500"></canvas>
</body>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.0/jquery.min.js"></script>
</html>
```

Onto `script.js`. Let's start by using jQuery to select the canvas and save it to a variable.

Next we need to set the canvas' **context**. In this case, we're going to set it to `"2d"` since we want to operate in that environment.

> There are a number of environments out there for 3D rendering, including "webgl" and "webkit-3d". If you were to use those, you would also need to link to the appropriate libraries.

```js
// script.js

let canvas = $("canvas")
canvas.getContext("2d")
```

## Let's Make a Game

<!-- TODOs -->
  <!-- Basic one/two-line definition -->
  <!-- Why would you use this for things that don't require canvas? -->
