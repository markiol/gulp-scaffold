## Install gulp

### 1.0 Install Node.JS:

[GitHub page manual](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)

### 1.1 Install gulp globally:

```
npm install -g gulp
```

### 1.2 Install gulp in your project devDependencies:

```
npm init
npm install --save-dev gulp
```

### 2. Create a `gulpfile.js` at the root of your project:

```
touch gulpfile.js
```

gulpfile.js:

```javascript
var gulp = require('gulp');

gulp.task('default', function(){
  // place code for your default task here
});
```

### 3. Run gulp

```
gulp
```

The default task will run and do nothing.

To run individual tasks, use `gulp <task> <othertask>`

## Where do I go now?

You have an empty gulpfile and everything is installed. How do you REALLY get started? Check out the [recipes and articles section](README.md#articles-and-recipes) for more information

## .src, .watch, .dest, CLI args - How do I use these things?

For API specific documentation you can check out the [documentation for that](API.md)

## Available Plugins

The gulp community is growing, with new plugins being added daily. See the [main website](http://gulpjs.com/) for a complete list.