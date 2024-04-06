## Start Creating Scss file for creating new CSS Themes ##

Created Readme.md by Gerard Yabut for step by step and for Learning and record every changes

## Updates Here!! ##

1. Install all dependencies and packages
    - npm init
    - install dart-sass
    - install bootstrap-v5
    - install font awesome
    - install autoprefixer sass

2. Go to package.json
    - Change the script to "compile:sass": "sass --watch scss:assets/css"
    - Add scss folder then create style.css file in it.
    - Add "start": "live-server"
    added sass --watch scss:assets/css so that we can check it and update realtime

3. Add Themingkit.html

4. Add _custom.scss in scss folder and add this
    - @import "../node_modules/bootstrap/scss/bootstrap.scss";

5. Go to scss/style.scss and use this code
    - @use 'custom';

6. Go to themingkit.html and add this 
    - <link rel="stylesheet" href="assets/css/style.css">

7. Edit the variable in _custom.scss
    - changing the primary colors and dropdown

8. Add some files partial files
    - components
        - _animations.scss
        - _buttons.scss
        - _mixins.scss
        - _typography.scss
    - sections
        - _navbar.scss
        - _intro-sections.scss
        - _companies.scss
        - _services.scss
        - _testimonials.scss
        - _portfolio.scss
        - _get-started.scss
        - _faq.scss
        - _footer.scss
9. Use Fontawesome icons
    - Add fontawesome.scsss and use from node modules
        - @use '../node_modules/@fortawesome/fontawesome-free/scss/ brands.scss';
        - @use '../node_modules/@fortawesome/fontawesome-free/scss/regular.scss';
        - @use '../node_modules/@fortawesome/fontawesome-free/scss/fontawesome.scss';
        - @use '../node_modules/@fortawesome/fontawesome-free/scss/solid.scss';
    - Copy webfonts folder from node_modules/@fortawesome/fontawesome-free to assets/scss.

10. you can now use and override varialbes from node_modules/bootstrap/_variables.scss

11. download glightbox
    - go to biati-digital.github.io/g/lightbox
    - download the source
    - go to dist folder and copy it.
    - create a new folder for vendors inside assets
    - create a new folder for glighbox and paste it inside.

12. add it to your html
    - link the css folder 'assets/vendors/glightbox/css/glightbox.css'
    - link the js folder 'assets/vendors/glightbox/js/glightbox.js

13. Add my custom Theme colors in _custom.scss
    - call @import '../node_modules./bootstrap/scss/functions'
    - call @import '../node_modules/bootstrap/scss/variables'
    - add your "custom-theme-color"
    - map-merge the the theme-colors and your custom-theme-colors