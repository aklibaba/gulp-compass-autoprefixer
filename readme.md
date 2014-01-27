### Install Node.js

* If Node is not yet installed on the machine, it will need to be [installed](http://nodejs.org/download/)


### Install Gulp

* If Gulp has never been set up on the machine, the gulp CLI will also need to be installed by running `npm install gulp -g`
* To install Gulp for the project (this only needs to happen once), switch to the root directory for the site in a terminal. For my configuration, you can install gulp and the dependencies using the command `npm install gulp-compass gulp-autoprefixer gulp-minify-css gulp-jshint gulp-concat gulp-uglify gulp-imagemin gulp-rename gulp-livereload tiny-lr gulp-cache --save-dev`. Again, you only need to do this once.
* Make sure and copy the gulp.js file to the base of your site. The provided gulp.js file is set up for the following file configuration

### Project Structure

* project root/
  * config/ ([Master Config](https://github.com/focuslabllc/ee-master-config) files)
  * html/ (web root)
    * css/
    * js/
    * images/
  * src/
    * js/
      * plugins.js
      * site.js
      * [various .js files]
    * scss/
      * [various .scss files]
      * styles.scss
  * system/ (EE system folder)
  * templates/ (EE templates)
  * gulpfile.js
  * package.json (will be added when gulp is installed via CLI)


### Run Gulp

* To just compile the scripts and SCSS one time, simply run the command `gulp`.
* To watch the templates, .scss, and .js files for changes, and to automatically compile and minify the relevant files, run the command `gulp live`. If the livereload browser extensions are installed and enabled, the browser will automatically refresh when any changes are made.



## Directory Structure