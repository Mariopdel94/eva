# Eva CSS

Theming is supported by changing the `settings.csss` file under `theme`. In there you can add your color palette, fonts, resolution breakpoints for easier media queries in your css rules in your project.

`bg-${color}-${variation}` classes are generated automatically and the contrasting text color assigned based on the [W3 color documentation guide](http://www.w3.org/TR/AERT#color-contrast) using the following formula:

```
((Red value X 299) + (Green value X 587) + (Blue value X 114)) / 1000
```