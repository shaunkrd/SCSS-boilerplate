# An SCSS Boilerplate #

Use as a starting point for any Sass/SCSS project. Designed as a time-saver and to provide enough CSS for a good, basic layout including handling of Flexbox grids. It uses Compass, but after a few tweaks the code will work well without it.

Some classes referenced in the CSS will be common in WordPress themes, and the CSS is designed to work particularly smoothly inside a WordPress theme.

### Installation ###

1. Clone the repo to your project directory. For example, if using in a WordPress theme then clone to the root of the theme directory. You will then have a 'src/scss' directory containing the parent 'styles.scss' file and the boilerplate SCSS partials.

2. Override the boilerplate CSS by using project specific partials and referencing them in 'styles.scss'. The order in which the project specific partials are referenced in 'styles.scss' is important. For example, the boilerplate 'variables.scss' partial contains variables for maximum page width, responsive breakpoints, default text colour and more. Override these with a project specific variables partial which must be referenced in 'styles.scss' *before* the boilerplate styles and layout partial which use the variables.

3. Use your favourite taskrunner to compile 'styles.scss' into a CSS file. I use Grunt and set my 'Gruntfile.js' to compile 'src/scss/styles.scss' into 'assets/css/styles.css' (which I also minify at the same time).

### Flexbox grids ###

Refer to the notes in 'flex-grids.scss' on how to control the presentation of elements within a grid using classes in the HTML.
