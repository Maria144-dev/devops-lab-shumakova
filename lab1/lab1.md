# Отчет по лабораторной №1

University: ITMO University  
Faculty: FTMI  
Course: introduction-in-web-tech  
Year: 2025/2026  
Group: U4225  
Author: Shumakova Maria  
Lab: Lab1 
Date of create: 07.10.2025
Date of finished: 07.10.2025

---
### Шаги выполнения

Установим докер с [официального сайта](https://www.docker.com/) и проверим его доступность в PS

![img](./img/image1.png)

Запускаем первый контейнер

![img](./img/image2.png)

Выполним поочередно `docker images`, `docker ps`, `docker ps -a` и посмотрим на результат

![img](./img/image3.png)

- `docker images` - выводит список образов, которые находятся на локальном хосте
- `docker ps` - отображает список активных контейнеров
- `docker ps -a` - отображает список всех контейнеров

Ставим образ Ubuntu и запускаем контейнер

![img](./img/image4.png)

В среде Ubuntu обновляем пакеты и ставим `curl`. Убедимся, что все хорошо

![img](./img/image5.png)

Запускаем контейнер с nginx и проверим локалхост на порту 8080

![img](./img/image6.png)  
![img](./img/image7.png)

Посмотрим логи контейнера и убедимся, что отобразилась ионфрмация о посещении

![img](./img/image8.png)

Проведем операции с контейнерами для закрепления материала  

- Посмотреть запущенные контейнеры: `docker ps`
- Посмотреть все контейнеры: `docker ps -a`
- Остановить контейнер: `docker stop web-server`
- Запустить остановленный контейнер: `docker start web-server`
- Удалить контейнер: `docker rm web-server`
- Удалить образ: `docker rmi nginx:alpine`

![img](./img/image9.png)  
![img](./img/image10.png)

Создадим том и запустим контейнер с ним, подключимся к контейнеру и создадим файл. Далее выходим, удаляем контейнер и создаем новый с таким же томом

![img](./img/image11.png)

Проверяем наличие файла

![img](./img/image12.png)
