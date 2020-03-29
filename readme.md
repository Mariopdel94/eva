# Eva CSS / SCSS

Eva is easily customizable for your needs. You can start using it right away, however you might want to change the color palette, fonts, breakpoints, spacing values, etc. This is fully customizable under the settings file.

You can even change the name of the project (which is used on some of the CSS Classes). So, instead of using the class eva-btn {}, you can change it for whatever prefix you like.

Theming is supported by changing the `settings.csss` file under `theme`. In there you can add your color palette, fonts, resolution breakpoints for easier media queries in your css rules in your project.

`bg-${color}-${variation}` classes are generated automatically and the contrasting text color assigned based on the [W3 color documentation guide](http://www.w3.org/TR/AERT#color-contrast) using the following formula:

```
((Red value X 299) + (Green value X 587) + (Blue value X 114)) / 1000
```

Eva also works with Angular Material and overrides some of their components with our own SCSS rules.

# Quick start

Several quick start options are available:

* Clone the repo: `git clone https://github.com/Mariopdel94/eva-css`
* Install with npm: `npm install eva-css`

Visit the [styleguide page](http://eva.mariopineda.com.mx/) for information on classes, rules, usage, etc.

**Note:** Eva uses the XY grid from Foundation 6.6.2. There's no need to install Foundation as the required files for the XY Grid are included in the installation.

# What's included

Inside the repo you'll find the following directories and files, logically grouping common assets. You'll see something like this:

```text
eva/
└── styles/
    ├── eva/
    │   ├── classes/
    │   |   ├── _button-classes.scss
    │   |   ├── _cards.scss
    │   |   ├── _color-classes.scss
    │   |   ├── _common.scss
    │   |   ├── _datepicker.scss
    │   |   ├── _flex.scss
    │   |   ├── _forms.scss
    │   |   ├── _snackbar.scss
    │   |   ├── _spacing.scss
    │   |   ├── _text.scss
    │   ├── _buttons.scss
    │   ├── _colors.scss
    │   ├── _responsive_.scss
    │   ├── _settings_.scss
    │   ├── eva-for-scss.scss
    │   └── eva.scss
    └── grid/
        ├── Foundation required files for XY Grid 6.6.2
```

# Installation

Once installed you need to import the base file on your main styles.

```scss
@import "~eva-css/styles/eva/eva.scss";
```

# Bugs and feature requests

Have a bug or a feature request? [Please open a new issue.](https://github.com/Mariopdel94/eva-css/issues/new)

# Creator

**Mario Pineda**

* [http://mariopineda.com.mx/](http://mariopineda.com.mx/)