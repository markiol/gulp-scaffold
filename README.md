## Вступление

#### Необходимые требования к участнику
	- Компьютер с доступом в интерент, email ящик;
	- Знать в достаточной степени: git, html, css, js.

#### Рекомендуемые требования
	- Компьютер с posix comand line интерфейсом;
	- Превосходно знать: git, html, css, js.
	- Текстовый редактор sublime text;

## Приступая к работе

### Для ознакомления
В проекте предполагается использовать npm, bower и gulp:
```
|--/bower_components // директория для компонентов bower
|--/node_moduled // директория для компонентов npm
|--bower.json
|--package.json
|--gulpfile.js
```
Для того чтобы использовать npm, bower и gulp потребуется установленый node.js
```
Node.JS >= 0.10.* 
npm >=1.4.3 
````
[О том как установить node.js](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)

Вести разработку на html, css, js не всегда удобно, поэтому используем предпроцессоры

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

О том как минимизиировать, сконкатинировать, и обфусцировать:
Для минимизации, сконкатининации, и обфускации будем использовать gulp;
А как именно написано [сдесь](http://habrahabr.ru/post/208890/)

### С этого момента можно присутпать

Я начну с создании деректорий под проект:
```
cd ~/Project
mkdir development development/scripts development/styles productions productions/fonts
```
Директории bower_components и node_moduled создавать не нужно, т.к. они сами будут создани.
Еще не нужно создавать bower.json и package.json, их лучше создать командой:
```
npm init
```
После ввода данной командыя я обычно выжимаю клавишу Enter до упора
Ошибок не возникает, выставляется по дефолту, если что можно отредактировать после

Сейчас поставим npm пакеты bower и gulp
```
npm install --save-dev bower gulp
```

Создавать gulpfile.js с содержимым:
`touch gulpfile.js`

содержимое gulpfile.js:

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