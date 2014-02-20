*This repository is a mirror of the [component](http://component.io) module [timoxley/canvas-noise](http://github.com/timoxley/canvas-noise). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/timoxley-canvas-noise`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# canvas-noise

  Generate noise on a canvas.

![https://raw.github.com/timoxley/canvas-noise/master/examples/example.png](https://raw.github.com/timoxley/canvas-noise/master/examples/example.png)

## Installation

    $ component install timoxley/canvas-noise

## Example

```js
var noise = require('canvas-noise')

// This generated the 8 images above

noise(canvas1)
noise(canvas2).grayscale()
noise(canvas3).opacity(1)
noise(canvas4).opacity(1).brightness(0.5)
noise(canvas5).brightness(0.2).opacity(1)
noise(canvas6).opacity(1).saturation(1)
noise(canvas7).saturation(1)
noise(canvas8).opacity(1).brightness(0.3).grayscale()

```

## API

### Noise#opacity(opacity:Number)

  Opacity of generated noise.

  Number between 0 and 1.

### Noise#saturation(saturation:Number)

  Saturation of generated noise.

  Number between 0 and 1.

### Noise#brightness(brightness:Number)

  Brightness of generated noise.

  Number between 0 and 1.

### Noise#grayscale()

  Enables grayscale mode. Randomises brightness instead of hue.

### Noise#color()

  Enables color mode. This is the default.
  Use this to disable grayscale mode.

### Noise#generate()

  Apply noise to canvas. Called implicitly on next tick on
  instantiation unless called explicitly.

  See animated example for more details on this.

## License

  MIT
