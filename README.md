## Getting Started

### System Requirements:

Node.JS >= 0.10.* 
npm >=1.4.3 

[GitHub manual page - Installing-Node.js](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)

### Installation gulp:

globally:

```
npm install -g gulp
```

in your project devDependencies:

```
npm install --save-dev gulp
```

### Create a `gulpfile.js`, 'dist/', 'build/' at the root of your project:

```
mkdir dist build
touch gulpfile.js
```

|--/bower_components // Components from bower
|--/build // Productions
|--|--/index.html
|--|--/styles.css
|--|--/scripts.js
|--/dist // Compiled components
|--|--/css
|--|--/fonts
|--|--/img
|--|--/js
|--/node_moduled // Components from npm
|--/not_compiled // Directory for development
|--|--/coffee
|--|--/less
|--|--/styles
|--|--/sass
|--package.json
|--gulpfile.js

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