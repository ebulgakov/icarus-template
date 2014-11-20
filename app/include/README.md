Includes
===============

## Настройка символических ссылок

Если верстка делается накомпьютере с Windows, то мои symlinks надо будет удалить, и подставить свои:
```sh
mklink /D bower_components C:\markup\project_html\app\bower_components
mklink /D css C:\markup\project_html\app\css
mklink /D js C:\markup\project_html\app\js
mklink /D img C:\markup\project_html\app\img
```
