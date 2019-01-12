# Section 04 - Gulp Essentials

## What is Gulp

  * A build system
  * A build tool
  * A task runner

There are a plethora of Gulp plugins to automate almost any task.


## Installing Gulp

Globally:

```
npm install gulp-cli --global
```


## Gulp in action

Gulp expects a `gulpfile.js`.

Example 

```
gulp.task('default', function() {
 ...
})
```

### gulp-watch

Watches the files on the filesystem and triggers a task when they change.

First import

```
var watch = require('gulp-watch');
```

Second, call within a task, passing two arguments. First is the name of the file to watch, second is a callback function.

```
  watch('./file-name', function() {...});
```


## Gulp and PostCSS

### gulp.src()

Pulls the source from the file.

### gulp.dest()

Puts the contents in the file.

### gulp.pipe()

Manipulates the content of the source file.

### Plugins used for Gulp

  * gulp-postcss
  * autoprefixer
  * postcss-simple-vars
  * postcss-nested

