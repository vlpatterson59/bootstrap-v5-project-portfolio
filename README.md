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
* implement glightbox using links and scripts:
```
    <link rel="stylesheet" href="assets/vendor/css/glightbox.min.css">
    <script src="assets/vendor/js/glightbox.min.js"></script>
    <script type="text/javascript">
        const lightbox = GLightbox({
            'href': 'https://www.youtube.com/watch?v=1PP-UTlh5wU',
            'type': 'video',
            'source': 'youtube', //vimeo, youtube or local
            'width': 900,
            'autoPlayVideos': 'true',
        });
    </script>
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
* create subfolders in the scss folder for *components* and *sections*
    * the *components* folder is for animations (_animations.scss), buttons (_buttons.scss), mixins (_mixins.scss), and typography (_typography.scss)
    * the *sections* folder is for the various web page sections (_navbar.scss, _services.scss, _testimonials.scss, etc)
* import the component files and section files into styles.scss using @use 'folder/filename'
* in each of the sections files, import the _custom.scss file using:
```
   @use '../custom' as *;
```
* use mixins (@mixin *name*) to define styles that can be re-used throughout the stylesheet (use @include *mixin-name* to utilize the mixin where needed)
    * include the mixins file (```@include '../components/mixins' as *;``` in the section file where the mixin is being used 
* to incorporate Font Awesome icons, create a *fontawesome.scss* file in the scss folder and include each of the brands:
    * ```@use '../node_modules/@fortawesome/fontawesome-free/scss/brands.scss';```
    * ```@use '../node_modules/@fortawesome/fontawesome-free/scss/regular.scss';```
    * ```@use '../node_modules/@fortawesome/fontawesome-free/scss/fontawesome.scss';```
    * ```@use '../node_modules/@fortawesome/fontawesome-free/scss/solid.scss';```
* for breakpoints, use ```@include media-breakpoint-up(*size*)``` or ```@include media-breakpoint-down(*size*)```
* 
## Resources and References

* [Node.js](https://nodejs.org/en/)
* [npm](https://www.npmjs.com/)
* [SASS](https://www.npmjs.com/package/sass)
* [Bootstrap](https://getbootstrap.com/)
    * [Positioning Utilities](https://getbootstrap.com/docs/5.0/utilities/position/)
* [Font Awesome](https://fontawesome.com/)
    * Secondary Font (CTA): [Font Awesome 5 Free](https://fontawesome.com/)
* [Autoprefixer](https://www.npmjs.com/package/autoprefixer)
* [Theming Kits](https://hackerthemes.com/kit/)
* [Google Fonts](https://fonts.google.com/)
    * Primary Font (Section Titles): [Poppins](https://fonts.google.com/specimen/Poppins?query=poppins)    
* [manypixels Free Illustration Gallery](https://www.manypixels.co/gallery)
* [Get Waves SVG shape generator](https://getwaves.io/)
* [GLightbox](https://biati-digital.github.io/glightbox/)