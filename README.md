Icarus пример развернутой верстки
===============

Пример установленного фреймворка [GeneratorIcarus] и рукводоство по пользованию

-


Если верстка будет работать на рабочей станции, то в Gruntfile.js
для connect:options:hostname поменять с 0.0.0.0 на localhost,а если на сервере, то ничего не менять

## Разворачивание сущестующей верстки

1. Зайти в директорию, где будет установлена верстка через консоль
2. Копируем адрес https://github.com/zoom-samara/icarus-template.git в консоль
3. Нажимаем Enter
4. Зайти в рабочую директорию через консоль
5. Набрать npm i
6. Набрать bower i

## Старт и деплой  верстки

    grunt serve - стартует верстку на 9000 порту
    grunt - тестирует верстку и компилирует её в /dist
    grunt build - сразу компилирует верстку в /dist

###Дополнительные ключи

    --force - работает в связке с serve, нужен, чтобы при ошибках сервер не вылетал
    --verbose - отладочный ключ. Работает со всеми командами. Если вы что-то сделали, но оно не работает. В отладочном режиме, можно посмотреть стек выполнения тасков


## Немного о самой верстке

* [Less/CSS]
* [Include]
* [Изображения]


### Другие директории
Директория "mocks" - эмулируют ответы с сервера



## ВАЖНО!
Все JS/CSS/HTML плагины устанавливать через bower с ключом --save

Пример установки jQuery:
```sh
bower i jquery --save
```
Все серверные плагины ставить через NPM с ключом --save-dev
Пример установки html-валидатора:
```sh
npm i grunt-html-validation --save-dev
```
## Дополнительная информация

Внутри отдельных модулей box, nav, form и т.д. можете писать, как считаете нужным.
Однако есть свои нюансы:

* классы без префикса вне элемента лежать не могут, это может создать угрозу потерять место, где лежит этот класс
* если элемент встречается на верстке больше одного раза – уводить его в include
* старайтесь по-максимуму уменьшить количество тегов в верстке

В изображениях:


## Плагины

### NPM Modules
Плагины используемы в проекте:
* grunt
* grunt-autoprefixer
* grunt-concurrent
* grunt-contrib-clean
* grunt-contrib-concat
* grunt-contrib-connect
* grunt-contrib-copy
* grunt-contrib-cssmin
* grunt-contrib-htmlmin
* grunt-contrib-imagemin
* grunt-contrib-jshint"
* grunt-contrib-less"
* grunt-contrib-uglify
* grunt-contrib-watch
* grunt-html-validation
* grunt-include-replace
* grunt-rev
* grunt-spritesmith
* grunt-usemin
* jshint-stylish
* load-grunt-tasks
* time-grunt

### jQuery Plugins
* [Twitter Bootstrap]
* [normalize.css] - Если не установлен Twitter Bootstrap
* [font-awesome]
* [modernizr]
* [jQuery]

## Todo's

 * Написать тесты
 * Добавить поддержку [AngularJS]
 * Добавить поддержку  [RequireJS]

## Если что-то пошло не так, как надо
Если вы обнаружили ошибку или хотите  добавить пожелание, есть два проверенных способа:

* Завести задачу в [Issues]
* Если вдруг не отвечаю,написать сразу на zoom81@ya.ru


License
----

MIT


**Free Software, Hell Yeah!**
[Issues]: https://github.com/zoom-samara/generator-icarus/issues
[Изображения]: https://github.com/zoom-samara/icarus-template/tree/master/app/img
[Include]: https://github.com/zoom-samara/icarus-template/tree/master/app/include
[Less/CSS]: https://github.com/zoom-samara/icarus-template/tree/master/app/css
[GeneratorIcarus]: https://github.com/zoom-samara/generator-icarus
[Yeoman]: http://yeoman.io/
[nodeJS]:http://nodejs.org
[Twitter Bootstrap]:http://twitter.github.com/bootstrap/
[jQuery]:http://jquery.com
[AngularJS]:http://angularjs.org/
[RequireJS]:http://requirejs.org/
[gruntJS]:http://gruntjs.com/
[normalize.css]: http://necolas.github.io/normalize.css/
[modernizr]:http://modernizr.com/
[font-awesome]: http://fontawesome.io/
