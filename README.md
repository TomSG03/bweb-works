## Задания по курсу «Работа веб-приложений»

- [x] [HTTP и современный Web. Формы и форматы передачи данных](https://github.com/TomSG03/bweb-works-http)
- [x] [JQuery](https://github.com/TomSG03/bweb-works-jquery)
- [x] [Bitrix JS](https://github.com/TomSG03/bweb-works-bitrixjs)
- [x] [REST](https://github.com/TomSG03/bweb-works-rest)
- [x] [JSON, XML](https://github.com/TomSG03/bweb-works-json)
- [x] [mySQL](https://github.com/TomSG03/bweb-works-mysql)
---

### Продление Демо - периода

В файле bitrix\modules\main\admin\define.php

заменяем строку на

define("TEMPORARY_CACHE", "ARtufgYHb2MMdQgebRtmG24A");

В таблице b_option поменять значение ключа admin_passwordh на FVgQeWYUBgQtCUVcBxcGCgsTAQ==

Сделать это можно через phpmyadmin руками или SQL запросом ниже:

UPDATE b_option SET VALUE = "FVgQeWYUBgQtCUVcBxcGCgsTAQ==" WHERE b_option.MODULE_ID = "main" AND b_option.NAME = "admin_passwordh";
Очистить папку bitrix/managed cache

Для удаления надписи в админке – правим файл \bitrix\modules\main\interface\prolog_main_admin.php 351 строка.

Находим echo BeginNote и делаем display:none как в примере ниже.

//echo BeginNote('style="position: relative; top: -15px;"');
echo BeginNote('style="display:none;"');


---
[Спискок курсов](https://github.com/TomSG03/Training-in-Netology)
