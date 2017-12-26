# VUI
### A dead simple (S)CSS framework

VUI (View User Interface, yeah that's the best I can do...) is a simple scss based ui kit. I really love other framework out there (bulma, angular material, uikit, etc...), but I prefer one that style direclty the dom's tags, without the clutter of wrapping them on a hell of tags (whenever possible obviously).

## [DEMO](https://kennyrulez.github.io/vui)

## Grid system
As I said, I love [Bulma](https://bulma.io "Bulma's Homepage") css framework, so I took from this project it's exceptional grid system.
It uses flexbox, like other projects ([gridlex](http://gridlex.devlint.fr) is one example, which I used before discovering bulma) and is very simple in it's basic flow. On advanced scenarios, it uses an intelligent naming system for classes to keep your code readable, so if in the future you will switch to another css framework, you can easily remeber your design choices and move without almost any pain.
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
./node_modules/vui/dist/vui.css
```
or
```sh
./node_modules/vui/vui.scss
```
to reference the scss version. Don't forget to compile!

## Documentation

I have not much time to write a proper documentation. Sorry for that. In [docs](docs) you can find a simple html page with all the tags this css styles and, whenever necessary, a brief explanation on why I used that particular way of code.

# Contributing
Fork the project and do your code! Then open a pull request. Please avoid to PR the `master` branch. Create a feature branch and PR that. I'll review and merge on the master.

## License
Code 2017 Valerio Fornito. Code released under [the MIT license](https://github.com/kennyrulez/vui/blob/master/LICENSE).
