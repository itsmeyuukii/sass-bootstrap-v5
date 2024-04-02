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
