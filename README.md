# VUI
### A dead simple (S)CSS ui kit

VUI (View User Interface, yeah that's the best I can do...) is a simple scss based ui kit. I really love other frameworks out there (bulma, angular material, uikit, spectre, etc...), but I prefer one that style directly the dom, without the clutter of wrapping them on a hell of tags (whenever possible obviously).

## [DEMO](https://kennyrulez.github.io/vui)

# 2018 Update
Added experimental navigationbar (horizontal only) with the classic hamburger when in mobile.

## Grid system
As I said, I love [Bulma](https://bulma.io) css framework, so I took from this project it's exceptional grid system.
It uses flexbox, like other projects ([gridlex](http://gridlex.devlint.fr) is one example, which I used before discovering bulma) and is very simple in it's basic flow. On advanced scenarios, it uses an intelligent naming system for classes to keep your code readable, so if in the future you will switch to another css framework, you can easily remember your design choices and move without almost any pain.
Please refer to bulma's documentation on columns system on https://bulma.io/documentation/columns/basics/.

## Normalize
The other library this project uses is [normalize.scss](https://github.com/JohnAlbin/normalize-scss) to normalize style behavior across the browsers. And I keep waiting for the day the gods of internet will drop support for IE.

# Installation
You can either download this project in your computer and reference it or use npm to install
```sh
npm install --save vui.scss
```
and use it in your project (plain css)
```sh
./node_modules/vui.scss/dist/vui.css
```
or
```sh
./node_modules/vui/src/vui.scss
```
to reference the scss version. Don't forget to compile!

# Variables
| Name                      | Description                   | Default       |
| --------------------------|------------------------------ | -------------:|
| $body-font                | font family for body          | sans-serif    |
| $body-line-height         | default line height for body  | 1.2           |
| $body-font-weight         | body font weight              | 300           |
| $heading-font             | heading (h1,h2...) font       | serif         |
| $heading-line-height      | heading line height           | 1.4           |
| $heading-font-weight      | heading font weight           | 500           |
| $font-color:              | default font color            | #333333       |
| $accent:                  | highlight color               | #2ca8ff       |
| $green:                   | green color (buttons, alert)  | #2ecc71       |
| $yellow:                  | yellow color (buttons, alert) | #f1c40f       |
| $orange:                  | orange color (buttons, alert) | #e67e22       |
| $red:                     | red color (buttons, alert)    | #cf2b1a       |
| $gray:                    | gray color (ui)               | CDCDCD        |

### Responsiveness breaks
| Name                      | Description                   | Default       |
| --------------------------|------------------------------ | -------------:|
| $mobile                   | when MQ breaks on mobile      | 35.5em        |
| $tablet                   | when MQ breaks on tablet      | 64em          |

### Variables for experimental features
| Name                      | Description                           | Default       |
| --------------------------|-------------------------------------- | -------------:|
| $nav-border-line          | navigationbar container border width  | 1px           |
| $nav-border-color         | navigationbar container border color  | 64em          |
| $arrow-color              | dropdown arrow color                  | 64em          |

## Documentation

I have not much time to write a proper documentation. Sorry for that. In [docs](docs) you can find a simple html page with all the tags this css styles and, whenever necessary, a brief explanation on why I used that particular way of code.

# Contributing
Fork the project and do your code! Then open a pull request. Please avoid to PR the `master` branch. Create a feature branch and PR that. I'll review and merge on the master.

## Many thanks to
[Bulma](https://bulma.io)

[normalize.scss](https://github.com/JohnAlbin/normalize-scss)

[Pure CSS Fancy Checkbox/Radio by Raúl Barrera](https://codepen.io/raubaca/pen/ONzBxP)

## License
Code 2017/2018 Valerio Fornito. Code released under [the MIT license](https://github.com/kennyrulez/vui/blob/master/LICENSE).
