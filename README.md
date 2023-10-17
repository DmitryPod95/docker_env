# docker_env

#Склонировать репозиторий Laravel
git clone https://github.com/laravel/laravel.git laravel

#Установить локально composer через docker
docker run --rm -v $(pwd):/app composer install

#Поменять права на папку с проектом
sudo chown -R $USER:$USER laravel

#Склонировать docker_env в папку с проектом
Выполнить команду docker-compose up -d

P.S подразумеваем, что Docker и Docker-compose установлены
