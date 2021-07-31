# yamdb_final
Проект спринта №19: YAMDB_FINAL

API для проекта YAMDB

http://84.252.143.105/

Установка Docker:
https://hub.docker.com/_/ubuntu

Клонирование репозитория:
git clone https://github.com/Dkobachevskiy/yamdb_final.git

Управление образами:
docker rmi - Удаляет образ, образ не может быть удален, если существуют контейнеры (даже незапущенные), которые основаны
на данном образе
Параметры:

-f - позволяет удалить образ даже если на нём основаны контейнеры
docker images - Отображает список всех существующих образов
Параметры:

-a | --all - отображает все образы (по умолчанию не отображает промежуточные контейнеры)
-q - отображает только id образов, вместо таблицы
Запуск и остановка контейнеров
docker run ОБРАЗ [КОМАНДА + АРГУМЕНТЫ] - Запускает выбранный образ в новом контейнере
Параметры:

-d | --detach - запускает контейнер в фоновом режиме и выводит только id свежесозданного контейнера. (по умолчанию == false)
-i | --interactive - запускает контейнер в интерактивном режиме (оставляет STDIN открытым, даже если контейнер запущен в неприкрепленном режиме)
-t | --tty - запускает псевдотерминал, часто используется с -i
-p | --publish=[] - пробрасывает порты контейнера в хост. Формат: ip:hostPort:containerPort | ip::containerPort | hostPort:containerPort | containerPort
-e | --env=[] - пробрасывает переменные окружения внутрь контейнера.
-v | --volume=[] - пробрасывает директорию файловой системы внутрь контейнера
docker stop КОНТЕЙНЕР - останавливает контейнер, передавая внутрь SIGTERM, а по истечении таймаута - SIGKILL


Команды для запуска приложения:
    source/venv/bin/activate
    pip install --upgrade pip
    pip install requirements.txt

Команду для создания суперпользователя:
    python manage.py createsuperuser

https://github.com/Dkobachevskiy/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg
