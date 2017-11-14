SVG Odometer Effect Library
======
> Crazy SVG odometer effect library. Library uses functional approach and ES7 Function Bind Syntax. Internals strongly inspired by d3.js library.

<p align="center"><img src ="docs/example.gif"/></p>

[Demo](https://coderitual.github.io/odoo/examples/)

Examples
======
The API is really simple and straigthforward:
```js
bounty.default({ el: '.js-bounty', value: '£42,000,000' });
```

You can use it with other **options**:
```js
bounty.default({
  el: '.js-bounty',
  value: '£42,000,000',
  initialValue: '£900,000',
  lineHeight: 1.35,
  letterSpacing: 1,
  animationDelay: 100,
  letterAnimationDelay: 100
});
```
If you want to **cancel** the ongoing animation just call returned function:
```js
const cancel = bounty.default({ el: '.js-bounty', value: '£42,000,000' });
cancel();
```

That's it?
=====
Yea! That's it. Other options like `font-family` and `font-size` are taken from **computed styles** so you can just style it like the other layers.
```css
.js-bounty {
  font-size: 60px;
  font-family: Roboto;
  fill: #fff;
  text-shadow: 1px 1px 5px rgba(0, 0, 0, 0.5);
}
```

Roadmap
====
There is a work in progress to implement additional features:
* `from` `to` API.
* Full ASCII transition support.
* Control animation.

<p align="center"><img src ="docs/example2.gif"/></p>

## License
The library is available under the MIT license. See the [LICENSE](LICENSE) file for more info.
