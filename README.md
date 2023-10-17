# docker_env

# шаг 1
Склонировать репозиторий Laravel
git clone https://github.com/laravel/laravel.git laravel

# шаг 2 
Установить локально composer через docker
docker run --rm -v $(pwd):/app composer install

# шаг 3 
Склонировать файлы docker_env в папку с проектом

# шаг 4 
Поменять права на папку с проектом
sudo chown -R $USER:$USER laravel

# шаг 5 
Скопировать файл .env.example
Переименовать в .env
Настроить под себя

# шаг 6
Выполнить команду docker-compose up -d

# шаг 7
нужно сгенерировать уникальный ключ приложения
docker-compose exec app php artisan key:generate

P.S подразумеваем, что Docker и Docker-compose установлены

# Сборка
php 8.1
mysql 5.7
nginx 
