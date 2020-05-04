### Шаблон для быстрого развертывания, для локально разработки

Для работы локально вам потребуется:
 - установить локальный сервер с php интерпретатором (https://www.apachefriends.org/ru/index.html) и запустить сервер
 - склонировать проект в папку htdocs на локальном сервере
 - установить composer (https://getcomposer.org/doc/00-intro.md)
 - установить git
 
## Запуск проекта

В корне проекта создать файл .env, скопировать в него все из файла .env.example, после чего выполнить команду ```php artisan key:generate ```

Запустить команду ```composer install```

Для запуска проекта выполнить команду ```php artisan serve```

## Запуск тестов

Запуск тестов:

```
vendor\bin\codecep run tests/acceptance
```

Для запуска других тестов, необходимо указать название другой директивы (unit, api и т. д.)

Запуск одного конкретного теста:

```
vendor\bin\codecep run tests/acceptance/ExampleCest.php:testSomething
```
