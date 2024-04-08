# Домашнее задание к занятию 15 «Система сбора логов Elastic Stack» - Семикова Т.В. FOPS-9

## Задание 1

Вам необходимо поднять в докере и связать между собой:

- elasticsearch (hot и warm ноды);
- logstash;
- kibana;
- filebeat.

Logstash следует сконфигурировать для приёма по tcp json-сообщений.

Filebeat следует сконфигурировать для отправки логов docker вашей системы в logstash.

В директории [help](./help) находится манифест docker-compose и конфигурации filebeat/logstash для быстрого 
выполнения этого задания.

Результатом выполнения задания должны быть:

- скриншот `docker ps` через 5 минут после старта всех контейнеров (их должно быть 5);
![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/1.jpg)
- скриншот интерфейса kibana;
![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/2.jpg)
- docker-compose манифест (если вы не использовали директорию help);
- ваши yml-конфигурации для стека (если вы не использовали директорию help).

## Задание 2

Перейдите в меню [создания index-patterns  в kibana](http://localhost:5601/app/management/kibana/indexPatterns/create) и создайте несколько index-patterns из имеющихся.

![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/3.jpg)

Перейдите в меню просмотра логов в kibana (Discover) и самостоятельно изучите, как отображаются логи и как производить поиск по логам.

![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/4.jpg)

![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/5.jpg)

![ad](https://github.com/SemikovaTV/hw_monitoring/blob/main/img_02/6.jpg)

---
