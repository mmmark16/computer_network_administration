# Лабораторная работа №1
**Выполнение**
- Создать файлы docker-compose.yml, promtail_config.yml
- Запустить compose файл командой `docker-compose up -d`
![image_2024-10-16_19-52-49](https://github.com/user-attachments/assets/d8a791ea-c63b-4d37-b811-8f51e14abb18)
- Создать администратора на nextcloud
  ![image_2024-10-16_19-58-55](https://github.com/user-attachments/assets/e8317542-1dfb-4c41-a85f-0d76e6cff250)
- Проверка логов neextcloud
  ![image_2024-10-16_20-09-10](https://github.com/user-attachments/assets/f3a2607b-f6da-41c6-81b2-cfb43a8c0984)
- Поднять Zabbix
  ![image_2024-10-16_20-14-27](https://github.com/user-attachments/assets/6972506e-cbc3-4c5a-9164-34668d465976)
- Добавить data source Loki
  ![image_2024-10-16_20-43-52](https://github.com/user-attachments/assets/50154aef-12a7-422a-b73c-45458119394e)
- Добавить data source Zabbix
  ![image_2024-10-16_20-44-42](https://github.com/user-attachments/assets/3c83cb6c-c978-4e6f-905f-623bc5d3081c)
- Создать дашборды на статус nextcloud и логи
![image_2024-10-16_20-55-11](https://github.com/user-attachments/assets/12817be5-0910-4fd2-8960-65d9d33edd09)
![image_2024-10-16_21-07-34](https://github.com/user-attachments/assets/7ab7bea5-7d5f-45dc-b4fc-2a31797cb968)

**Ответы на вопросы**
- SLO и SLA: в чём разница?  
SLO (Service Level Objective) — это цель и ожидаемый уровень доступности сервиса, который в идеале должен быть достигнут.  
SLA (Service Level Agreement) — это соглашение, где прописаны конкретные параметры качества обслуживания. Тут могут быть указаны различные метрики для измерения уровня доступности и производительности сервиса и, возможно, санкции за несоблюдение SLO  

- Инкрементальный и дифференциальный бэкап: в чём отличие?  
Инкрементальное резервное копирование — копирования происходит только тех файлов, которые были изменены после любого последнего копирования. Таким образом сокращается время и объем данных для копий  
Дифференциальное резервное копирование копирует все данные, изменённые после последнего полного копирования.  

- Мониторинг и observability: в чём различие?  
Мониторинг — это сбор и анализ данных о работе системы. Он нужен, чтобы понять, что возникла проблема, но не получится узнать первопричину.  
Observability — это более широкий подход, который включает в себя мониторинг, а также логирование и другие методы сбора информации.
Observability позволяет получить более полное представление о том, что происходит внутри системы, и выявить, почему именно возникла та или иная проблема
