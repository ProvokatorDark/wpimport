﻿ОПИСАНИЕ
---------

Плагин предназначен для Переноса данных из WordPress в LiveStreet

Для настройки необходимо записать правильные параметры для доступа к БД
WordPress:
```
    $config['wpdb'] = 
        array(
            'type'=>'mysql',
            'user'=>'',
            'pass'=>'',
            'host'=>'localhost',
            'port'=>'3306',
            'dbname'=>''
            );
```
Импорт происхдит через админку: http://livestreet/wpimport/admin
Импортируются отдельно Пользователи, Категории, Топики и коментарии.
Существует возможность импорта отдельных топиков.

Также присутствует механизм импорта посредством перехода на страницы 
(особенно важно для того, чтобы не потерять трафик). Ипморт происходит 
на лету при переходе по старому адресу.

В данный момент плагин находится в бета-тестировании.
Уже был использован на сайтах:
    * http://koko.by/,
    * http://protiv-ugona.ru/,

ОСТОРОЖНО
---------

Во избежании недоразумений, перед импортом обязательно делать резервную копию БД.
Если у Вас есть индивидуальные пожелания по импорту, то можно написать мне личное сообщение
http://livestreet.ru/profile/1099511627776/ сюда
