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

* [HTML]
* [Less/CSS]
* [Include]
* [Изображения]
* [Mocks]
* [Dist] - по-умолчанию в .gitigore. Директория с собранным проектом. Обычно для него делается своя ветка в git-репозитории 


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
* grunt-contrib-jshint
* grunt-contrib-less
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


License
----

MIT


**Free Software, Hell Yeah!**
[HTML]: https://github.com/zoom-samara/icarus-template/tree/master/app
[Mocks]: https://github.com/zoom-samara/icarus-template/tree/master/app/mocks
[Dist]: https://github.com/zoom-samara/icarus-template/tree/master/dist
[Issues]: https://github.com/zoom-samara/generator-icarus/issues
[Изображения]: https://github.com/zoom-samara/icarus-template/tree/master/app/img
[Include]: https://github.com/zoom-samara/icarus-template/tree/master/app/include
[Less/CSS]: https://github.com/zoom-samara/icarus-template/tree/master/app/css
[GeneratorIcarus]: https://github.com/zoom-samara/generator-icarus
[Yeoman]: http://yeoman.io/
[nodeJS]:http://nodejs.org
[Twitter Bootstrap]:http://twitter.github.com/bootstrap/
[jQuery]:http://jquery.com
[gruntJS]:http://gruntjs.com/
[normalize.css]: http://necolas.github.io/normalize.css/
[modernizr]:http://modernizr.com/
[font-awesome]: http://fontawesome.io/
