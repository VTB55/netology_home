Ответы на домашнее задание к занятию 4 «Оркестрация группой Docker контейнеров на примере Docker Compose»:

Задача 1:

https://hub.docker.com/repository/docker/konovalovs/custom-nginx/general

Задача 2:

<img width="702" height="770" alt="image" src="https://github.com/user-attachments/assets/b85e212d-a1a1-4f53-98e0-f4c93e8b1447" />
<img width="1377" height="878" alt="image" src="https://github.com/user-attachments/assets/0e78baa9-7376-49a1-ae56-f6aa9d806e5d" />

Задача 3:

<img width="2039" height="799" alt="image" src="https://github.com/user-attachments/assets/3f2c7dbc-ab06-4e33-a7f4-5184f8fc2d60" />
<img width="2057" height="814" alt="image" src="https://github.com/user-attachments/assets/96f586c2-31f8-4229-86cc-5603b5b05f41" />

Задача 4:

<img width="1164" height="1285" alt="image" src="https://github.com/user-attachments/assets/39e0437a-d879-4148-a64d-b004587ee382" />
<img width="1165" height="1277" alt="image" src="https://github.com/user-attachments/assets/fe0f8045-0977-473b-b74e-b5fbb6d2d8cb" />
<img width="1168" height="1280" alt="image" src="https://github.com/user-attachments/assets/a5736a12-fe46-4900-aee0-4f88bc403a8f" />

Задача 5:

Создайте отдельную директорию(например /tmp/netology/docker/task5) и 2 файла внутри него. "compose.yaml" с содержимым:

<img width="978" height="128" alt="image" src="https://github.com/user-attachments/assets/67472a7c-cbd8-4e03-9799-069c9795366e" />

И выполните команду "docker compose up -d". Какой из файлов был запущен и почему?

<img width="979" height="271" alt="image" src="https://github.com/user-attachments/assets/8b12c3f6-3e5b-4912-be68-889218c259f0" />

После выполнения команды docker-compose up -d в директории /tmp/netology/docker/task5 был запущен файл docker-compose.yaml.
Почему: В системе на данный момент используется старый Docker с отдельным бинарником docker-compose (и применяется через дефис), который ищет файлы в следующем порядке приоритета: 
docker-compose.yml, docker-compose.yaml, compose.yml, compose.yaml

Отредактируйте файл compose.yaml так, чтобы были запущенны оба файла:


