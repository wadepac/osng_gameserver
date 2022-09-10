
## Описание директорий 

> При скачивании сохраните структуру директорий.

### Panel

В этой директории содержится конфигуарция docker-compose для основной панели игрового сервера.

### Wings

В этой директории содержится конфигурация docker-compose для серверной части.


## Заметки по последовательности действий

1.	Выполнить конфигурацию основной панели и настроить web-доступ
2.	Выполнить конфигурацию серверной части
3.	Сконфигурировать игру


## Конфигурация основной панели.

Вам необходимо следуя ТЗ изменить файл docker-compose под требования вашего начальства.

Для запуска используйте стнадартную команду с указанием флага для скрытого вывода.

Для создания дополнительных пользователей используйте команду:
 < docker compose run --rm panel php artisan p:user:mak >

Доступ до web осуществляется с помощью данных, указанных в конфигурации с созданным пользователем.

## Конфигурация серверной части.

Для начала вам надо с помощью web-доступа добавить новый Location с именем **srvnodes**.

Далее так же с помощью web-доступа добавить новую ноду с указанными в ТЗ параметрами.

Отредактируйте по указанным в ТЗ параметрам файлы игрового сервера, запустите так же с флагом скрытого вывода в соответствующей директории.
Во вкладке конфигурации ноды выберите **Configuration** и следуйте указаниям платформы для полной конфигурации рабочей ноды.

Когда нода сконфигурирована во вкладке **Allocation** создайте новый следуя ТЗ.

## Конфигурация игрового сервера  с игрой

Во вкладке **servers** создайте новый и сконфигурируйте с параметрами, указанными в ТЗ. 
После создания откройте в новом окне терминал и иницируйте установку.

Если вы все сделаете правильно - Ваш сервер будет работать и вы сможете поиграть.
