# Portfolio Template built with Bootstrap 5 and SASS

This is a project from [freeCodeCamp](https://www.freecodecamp.org)'s YouTube channel. The course is [Learn Bootstrap 5 and SASS by Building a Portfolio Website - Full Course](https://www.youtube.com/watch?v=iJKCj8uAHz8) presented by Patrick Muriungi of [VAXA Digital](https://vaxadigital.com/).

This project was started June 30, 2021 and completed July 7, 2021.

The objective of this project was to create a single-page portfolio web template utilizing Bootstrap 5 and SASS. Features include a fixed navigation bar, 'waves' to separate the various sections of the page, button animations, a video library 
## Modifications and Enhancements

## What I Learned

* installing Node.js
* using npm init to create a package.json file \(start time: 4m30s; end time: 6m55s\)
* installing SASS using the command line:
```
    npm install --save-dev sass
```
* installing Bootstrap using the command line:
```
    npm install bootstrap --save
```
* installing Font Awesome using the command line:
```
    npm install --save @fortawesome/fontawesome-free
```
* installing autoprefixer using the command line:
```
    npm install postcss-cli autoprefixer --save
```
* edit "scripts" in package.json:
```
    "compile:sass": "sass --watch scss:assets/css"
```
* start the script from the command line:
```
    npm run compile:sass
```
* create a _custom.scss file in the scss folder for any custom variables
* import bootstrap.scss into _custom.scss with the following statement:
```
    @import "../node_modules/bootstrap/scss/bootstrap.scss";
```
* use the _custom.scss file in the style.scss file with the following statement:
```
    @use 'custom';
```
* Bootstrap SASS variables can be found in node_modules/bootstrap/scss/_variables.scss
* create subfolders in the scss folder for components and sections
    * the *components* folder is for animations (_animations.scss), buttons (_buttons.scss), mixins (_mixins.scss), and typography (_typography.scss)
    * the *sections* folder is for the various web page sections (_navbar.scss, _services.scss, _testimonials.scss, etc)
## Resources and References

* [Node.js](https://nodejs.org/en/)
* [npm](https://www.npmjs.com/)
* [SASS](https://www.npmjs.com/package/sass)
* [Bootstrap](https://getbootstrap.com/)
* [Font Awesome](https://fontawesome.com/)
* [Autoprefixer](https://www.npmjs.com/package/autoprefixer)
* [Theming Kits](https://hackerthemes.com/kit/)