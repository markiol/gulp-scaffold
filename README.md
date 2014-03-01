## Приступая к работе

### Архитектура предполагаемого проекта
В проекте предполагается использовать bower и npm, и т.д.:
```
|--/bower_components // компоненты bower
|--/node_moduled // компоненты npm
```
Вести разработку предполагается в scripts/ и styles/ на чем угодно:
```
|--/development
|--|--/scripts
|--|--|--script.js
|--|--|--script.coffee
|--|--/styles
|--|--|--style.css
|--|--|--style.less
|--|--|--style.styles
```
На выходе(сдача проекте), предполагается получить полностью готовый продукт*:
```
|--/productions
|--|--/index.html
|--|--/styles.css
|--|--/scripts.js
|--|--/fonts
|--|--|--/fonts.eot
|--|--|--/fonts.svg
|--|--|--/fonts.ttf
|--|--|--/fonts.woff
```
готовый продукт* - значит минимизиированый, сконкатинированый, обфусцированый

**Пару слов о шрифтах:**
*Разные типы шрифтов поддерживаются разными браузерами.*
*Универсального формата, увы, нет. Приходится держать пачку файлов.*

*Со шрифтами еще не известно все, пока пусть будет так(оставим этот момент).*

[Посмотрите ввидео о языке разметки Markdown *рус*](http://www.youtube.com/user/ArtSorax?feature=watch)

[Тест пишу и спользоанием разметки md](https://help.github.com/articles/markdown-basics)
Дальше текст неотформатированый, проссто накидано всякой ерунды, можете не читать...
```
|--/dist // Compiled components (non min)
|--|--/css
|--|--/fonts
|--|--/img
|--|--/js
|--package.json
|--gulpfile.js
```

### System Requirements:

```
Node.JS >= 0.10.* 
npm >=1.4.3 
````
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