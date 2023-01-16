# DXOpal

Game development framework for [Opal](https://opalrb.com/),
has similar API to [DXRuby](http://dxruby.osdn.jp/)

## Demo

- [triangles game in Ruby](https://code4fukui.github.io/dxopal-es/examples/es/triangles.html)
- [call JavaScript function from Ruby](https://code4fukui.github.io/dxopal-es/examples/es/)

## How to use

see https://yhara.github.io/dxopal/

```html
<canvas id="dxopal-canvas"></canvas>
<script type="module">
import { Opal } from "https://code4fukui.github.io/dxopal-es/build/dxopal.js";
eval(Opal.compile(`require 'dxopal'
Window.load_resources do
  Window.loop do
    x = Window.width / 2
    y = Window.height / 2
    dx = 72
    dy = 50
    Window.draw_triangle_fill(
      x, y - dy,
      x - dx, y + dy,
      x + dx, y + dy,
      [255, 255, 0]
    )
  end
end
`));
</script>
```
([RUN on ES-Jam](https://code4fukui.github.io/htmlprac/?url=https://code4fukui.github.io/dxopal-es/examples/es/simple.html))

## License

MIT (including images and sounds under examples/)

## Acknowledgements

- [Opal](https://opalrb.com/)
- [DXRuby](http://dxruby.osdn.jp/)
- [Bxfr](https://www.bfxr.net/) examples/apple_catcher/sounds/Explosion2.wav is made by this

## Contact

https://github.com/yhara/dxopal
