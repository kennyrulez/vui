# VUI

## This packages is deprecated. Please move to a better, modern css framework like bulma or my new favorite tool, tailwind css.

### A dead simple (S)CSS ui kit

VUI (View User Interface, yeah that's the best I can do...) is a simple scss based ui kit. I really love other frameworks out there (bulma, angular material, uikit, spectre, etc...), but I prefer one that style directly the dom, without the clutter of wrapping them on a hell of tags (whenever possible obviously).

## [DEMO](https://kennyrulez.github.io/vui)

# 2018 Update

## 0.5.2

Tweaks on form tag and select tag for a more consistent view

## 0.5.1

Small fixes on alignments for navigation bar

## 0.5.0

Updated the navigation bar, to be more solid on mobile. Removed the surrouding lines around, modified the hamburger menu (now colorable).

Now svgs do not require special char, just insert the color you want, sass will take care of the rest.

Fixed the notification popup in mobile view.

Updated to bulma grid system 0.7.1 [ChangeLog](https://github.com/jgthms/bulma/blob/master/CHANGELOG.md)

## 0.4.4

Removed the `$font-color` variable, it was useless.
Notification now have a better naming convention, using top, bottom, left, right. So if you need to show your notification on the top right of the page, use
`<div class="notification-container top right">`
Default margin from the page is 10px. Please edit `$notification-margin` accordingly.

## 0.4.3

Added equal column widths on table using flexbox.
Now checkboxes and radios have the same color schema as buttons

## 0.4.2

Updated Bulma columns to 0.7.0. Please read their [ChangeLog](https://github.com/jgthms/bulma/blob/master/CHANGELOG.md) for up-to-date info about.

## 0.4.1

Small bug fixes

## 0.4.0

Some tweaks for notification bar: now the position is fixed, so even if you scroll the bar remain visibile.
Now it views better on mobile, and has some new MQ on other screen resolutions.
**ATTENTION**: I renamed the Media Queries `mq-mobile` and `mq-tablet` to new names, so these changes will break compilation if your project use these varabiles. Please adjust accordingly (View 'Variables' later in this document).

## 0.3.5

(yeah, 0.3.4 was a refining release, not enough to have a description)
Added responsive table, with some quirks. Thanks StackOverflow for pointing me in the right directions using `data-` html attributes.

## 0.3.3

Added experimental notification popup with css transition. I've included a simple javascript to show/hide the popup. Use your own in your project.

## 0.3.2

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

[nodemon] starting `npm run build`
or
[nodemon] starting `npm run build`

```sh
[nodemon] starting `npm run build`
./node_modules/vui.scss/src/vui
[nodemon] starting `npm run build`
```

[nodemon] starting `npm run build`
to reference the scss version. Don't forg
[nodemon] starting `npm run build`et to compile!

[nodemon] starting `npm run build`

# Variables

[nodemon] starting `npm run build`
To edit one or more variable, import in y
[nodemon] starting `npm run build`our scss

```sh
./node_modules/vui.scss/src/_settings
```

and redefine one of following variables:

| Name                 | Description                   |    Default |
| -------------------- | ----------------------------- | ---------: |
| $body-font           | font family for body          | sans-serif |
| $body-line-height    | default line height for body  |        1.2 |
| $body-font-weight    | body font weight              |        400 |
| $heading-font        | heading (h1,h2...) font       |      serif |
| $heading-line-height | heading line height           |        1.4 |
| $heading-font-weight | heading font weight           |        500 |
| $accent:             | highlight color               |    #2ca8ff |
| $green:              | green color (buttons, alert)  |    #2ecc71 |
| $yellow:             | yellow color (buttons, alert) |    #f1c40f |
| $orange:             | orange color (buttons, alert) |    #e67e22 |
| $red:                | red color (buttons, alert)    |    #cf2b1a |
| $gray:               | gray color (ui)               |    #cdcdcd |

### Responsiveness breaks

changed in 0.4.0

| Name     | Description                          | Default |
| -------- | ------------------------------------ | ------: |
| $mq-568  | when MQ breaks on mobile             |  35.5em |
| $mq-768  | when MQ breaks on tablet (landscape) |  35.5em |
| $mq-1024 | when MQ breaks on tablet             |    64em |
| $mq-1280 | when MQ breaks on laptop             |    80em |

### Variables for experimental features

#### Navigation bar

| Name                  | Description                    | Default |
| --------------------- | ------------------------------ | ------: |
| $nav-hamburger-color  | Hamburger color                | #cf2b1a |
| $nav-arrow-color      | dropdown arrow color           | #e67e22 |
| $nav-hover-color      | color when hovering items      | #2ecc71 |
| $nav-text-color       | items text color               | #2ca8ff |
| $nav-text-hover-color | items text color when hovering |    #fff |

#### Notification

changed in 0.4.4

| Name                        | Description                              |         Default |
| --------------------------- | ---------------------------------------- | --------------: |
| $notification-font-size     | font size                                |           .85em |
| $notification-width         | width of the notification                |             30% |
| $notification-width-tablet  | width of the notification in tablet mode |             70% |
| $notification-width         | width of the notification in latpop mode |             30% |
| $notification-margin        | margin                                   |            10px |
| $notification-border-radius | container border radius                  |            10px |
| $notification-transition    | appear transition                        | .8s ease-in-out |
| $notification-default-color | default color                            |         #cdcdcd |

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
