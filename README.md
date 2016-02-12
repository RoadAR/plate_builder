# VLC rtsp streamer

## Установка vagrant

Скачать и поставить [vagrant](https://www.vagrantup.com/)

Скачать и поставить [virtualbox](https://www.virtualbox.org/)

Для убунты и других линуксов есть соответствующие пакеты

## Загрузка бокса

`vagrant box add alt6 alt6.box`

## Структура папок

Предполагается что этот Vagrantfile лежит на директорию выше, чем проект plate-recognition, таки побразом получается такая иерархия

```
cache  crop  pipeline-log  plate-recognition  plates  plates_cache  Vagrantfile  video
```

## Запуск и сборка
`vagrant up`

Вход в бокс

`vagrant ssh`

Сборка

```
# cd /vagrant/plate-recognition
# make
# ./bundle.sh
```

После этого в папке bundle будет полностью изолированная сборка со всеми зависимостями, требудет правки config.ini внутри

## Остановка бокса

`vagrant halt` или `sudo poweroff` внутри бокса
