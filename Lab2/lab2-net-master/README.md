Лабораторная работа №2

Инсталляция ansible
<img width="764" alt="Снимок экрана 2024-11-07 в 19 49 01" src="https://github.com/user-attachments/assets/c92fb3d2-61c1-4c1e-8fb5-0b0dd41a03ae">

Создаем базовый конфиг файл, затем папку inventory и в ней файл с хостами 
<img width="762" alt="Снимок экрана 2024-11-07 в 19 51 05" src="https://github.com/user-attachments/assets/31f7634a-a0cb-4fb7-bd9d-5ec24fdcc195">

Проверяем, что сервер с Ansible подключился к “клиенту”
<img width="765" alt="Снимок экрана 2024-11-07 в 19 51 52" src="https://github.com/user-attachments/assets/d4d26923-980e-49ec-ba8f-4b3606556081">

Создаем текстовый файл с производным содержимым, через модуль shell
<img width="1175" alt="Снимок экрана 2024-11-07 в 19 53 08" src="https://github.com/user-attachments/assets/ae39845d-a05f-4862-9850-d869e9541b87">

Удаляем файл через модуль file
<img width="1109" alt="Снимок экрана 2024-11-07 в 19 53 45" src="https://github.com/user-attachments/assets/c3792484-2122-47ca-bd67-a9f5ded1f004">

Создадим в рабочей директории папку roles и в ней инициализируем исходное конфигурационное дерево: ansible-galaxy init caddy_deploy
<img width="841" alt="Снимок экрана 2024-11-07 в 19 56 55" src="https://github.com/user-attachments/assets/55c09b89-e4c0-4da0-bb56-ddc29e747a2b">

 В рабочей директории создаем файл конфигурации самого плейбука, где указываем нужные нам хосты и роли
<img width="816" alt="Снимок экрана 2024-11-07 в 19 59 54" src="https://github.com/user-attachments/assets/06e113fa-76b9-47e6-a751-acfcc1fdd096">

Запускаем плейбук
<img width="1250" alt="Снимок экрана 2024-11-07 в 20 02 52" src="https://github.com/user-attachments/assets/22897967-4081-452f-aa28-36eaa703ced7">

Создадим шаблон (Jinja2), добавляем плейбук новые шаги, отвечающие за создание конфигурационного файла из шаблона и последующую перезагрузку сервиса. 
Проверяем, что страничка Caddy автоматически поднялась на подписанном сертификате с https
<img width="916" alt="Снимок экрана 2024-11-07 в 20 10 35" src="https://github.com/user-attachments/assets/3fb2dd6a-94e9-49b8-89c6-16bcfeed4955">
<img width="1250" alt="Снимок экрана 2024-11-07 в 20 19 18" src="https://github.com/user-attachments/assets/77672357-a4c8-4d45-97db-f1fedf657462">
<img width="1151" alt="Снимок экрана 2024-11-07 в 20 26 14" src="https://github.com/user-attachments/assets/73973ed5-5253-46fa-a33b-de6c1f0d7f71">
<img width="1148" alt="Снимок экрана 2024-11-07 в 20 32 33" src="https://github.com/user-attachments/assets/99ec5f7b-5cff-4820-86ff-9bb6acc5d1d8">


Задание №1
<img width="556" alt="Снимок экрана 2024-11-07 в 20 56 03" src="https://github.com/user-attachments/assets/aa5add18-710f-47ba-9426-6660233e2e80">
<img width="1252" alt="Снимок экрана 2024-11-07 в 20 56 43" src="https://github.com/user-attachments/assets/dd50163e-3f16-49db-ac4d-785dff3b15f3">

Задание №2
<img width="841" alt="Снимок экрана 2024-11-07 в 21 14 40" src="https://github.com/user-attachments/assets/ecba2367-8a89-4bde-afe8-9ec1671400b9">
<img width="484" alt="Снимок экрана 2024-11-07 в 21 14 49" src="https://github.com/user-attachments/assets/a1cb4360-f70b-4164-991b-b5c1309f793d">

Ура, все работает
<img width="497" alt="Снимок экрана 2024-11-07 в 21 15 20" src="https://github.com/user-attachments/assets/d2924cf5-b700-454f-87b9-8936b39d66da">
