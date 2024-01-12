# Домашнее задание к занятию «Система мониторинга Zabbix»
### Задание 1 

Установите Zabbix Server с веб-интерфейсом.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите PostgreSQL. Для установки достаточна та версия, что есть в системном репозитороии Debian 11.
3. Пользуясь конфигуратором команд с официального сайта, составьте набор команд для установки последней версии Zabbix с поддержкой PostgreSQL и Apache.
4. Выполните все необходимые команды для установки Zabbix Server и Zabbix Web Server.

#### Требования к результаты 
1. Прикрепите в файл README.md скриншот авторизации в админке.
2. Приложите в файл README.md текст использованных команд в GitHub.

### Решение 1
1. Работающий сервис:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/0.png)
2. Вход в админку:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/4.png)
3. Работающий вебинтерфейс:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/1.png)

4. Для установки использовались инструкции с офф сайта для ubuntu 22. Так же пришлось немного поколодовать с php, который был ранее установлен в рамках других дз и не правильно воспринимался апачем. Инструкции взяты отсюда: https://www.zabbix.com/ru/download?zabbix=6.0&os_distribution=ubuntu&os_version=22.04&components=server_frontend_agent&db=pgsql&ws=apache

### Задание 2 

Установите Zabbix Agent на два хоста.

#### Процесс выполнения
1. Выполняя ДЗ, сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 вирт.машины, одной из них может быть ваш Zabbix Server.
3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов.
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera.
5. Проверьте, что в разделе Latest Data начали появляться данные с добавленных агентов.

#### Требования к результаты 
1. Приложите в файл README.md скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу
2. Приложите в файл README.md скриншот лога zabbix agent, где видно, что он работает с сервером
3. Приложите в файл README.md скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.
4. Приложите в файл README.md текст использованных команд в GitHub

### Решение 2

1. Запущенный сервис агента на сервере:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/2.png)
2. Запущеннный сервис агента на второй машине:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/3.png)
3. Список хостов виден тут:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/1.png)
4. Получаемые данные с сервера:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/5.png)
5. Получаемые данные с клиента:
   ![img](https://github.com/valery-dubinin/zabbix_hw1/blob/main/6.png)   
   
