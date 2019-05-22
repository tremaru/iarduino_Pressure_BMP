
[![](https://iarduino.ru/img/logo.svg)](https://iarduino.ru)[![](https://wiki.iarduino.ru/img/git-shop.svg?3)](https://iarduino.ru) [![](https://wiki.iarduino.ru/img/git-wiki.svg?2)](https://wiki.iarduino.ru) [![](https://wiki.iarduino.ru/img/git-lesson.svg?2)](https://lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2)](http://forum.trema.ru)

# iarduino_Pressure_BMP [СКАЧАТЬ](https://github.com/tremaru/iarduino_Pressure_BMP/archive/master.zip)
Библиотека iarduino_Pressure_BMP позволяет считывать температуру окружающей среды и атмосферное давление с датчиков [BMP180](http://iarduino.ru/shop/Sensory-Datchiki/barometr-gy-68-datchik-atmosfernogo-davleniya-bmp180.html) и [BMP280](http://iarduino.ru/shop/Sensory-Datchiki/barometr-trema-modul.html), а так же рассчитывать высоту.

> Подробнее про установку библиотеки читайте в нашей [инструкции](https://wiki.iarduino.ru/page/Installing_libraries/).

Пример подключения к [Arduino](https://iarduino.ru/shop/boards/arduino-uno-r3.html)/[Piranha UNO](https://iarduino.ru/shop/boards/piranha-uno-r3.html) с помощью [Trema Shield](https://iarduino.ru/shop/Expansion-payments/trema-shield.html)
Подробнее о [подключении модуля](https://wiki.iarduino.ru/page/trema-modul-pressure-meter) 
![enter image description here](https://iarduino.ru/img/upload/ff71929a63d941fd58dc5a60860d0671.png)

| Модель | Ссылка на магазин|
|--|--|
| Красная ![enter image description here](https://wiki.iarduino.ru/img/resources/840/840.svg) | https://iarduino.ru/shop/Displei/chetyrehrazryadnyy-indikator-led-trema-modul.html|
| BMP180 ![enter image description here](https://wiki.iarduino.ru/img/resources/840/840.svg) | https://iarduino.ru/shop/Displei/chetyrehrazryadnyy-indikator-led-zelenyy-trema-modul.html |

## Описание библиотеки:
Библиотека позволяет регулировать яркость свечения LED индикатора, выводить на него числа (целые, дробные, положительные, отрицательные), символы ("abcdefghijlnopstu .,:;*-_"), массивы чисел, время и температуру.
**[  Подробное описание, подключение и примеры работы ](https://wiki.iarduino.ru/page/chetyrehrazryadnyy-indikator-trema-modul/)**

## Назначение функций и переменных:
Подробное описание работы с библиотекой, находится в разделе [Wiki Четырёхразрядный индикатор](https://wiki.iarduino.ru/page/chetyrehrazryadnyy-indikator-trema-modul/ "Wiki Четырёхразрядный индикатор").

**Подключаем библиотеку.**

    #include <iarduino_4LED.h> // Подключаем библиотеку.
    
**Создаём объект.** 

    iarduino_4LED ОБЪЕКТ ( ВЫВОД_CLK , ВЫВОД_DIO ); // Создаём объект.

**Инициализация работы с LED индикатором.**

    Функция begin(); // Инициализация работы с LED индикатором.
    
**Очистка индикатора (выключение всех сегментов).**

    Функция clear(); // Очистка индикатора (выключение всех сегментов).
    
**Установка яркости свечения индикатора, от 0 до 7.**

    Функция light( ЧИСЛО ); // Установка яркости свечения индикатора, от 0 до 7.
    
**Управление точками на индикаторе.**

    Функция point( ПОЗИЦИЯ , СОСТОЯНИЕ ); // Управление точками на индикаторе.
    
**Вывод значения на индикатор.**

    Функция print( ЗНАЧЕНИЕ [ , ПАРАМЕТРЫ_ВЫВОДА_ЧИСЛА ] ); // Вывод значения на индикатор.
    
**Устанавливает светодиоды (сегменты) индикатора по битам.**

    Функция setLED( [[[[[ БАЙТ_№1 ] , БАЙТ_№2 ] , БАЙТ_№3 ] , БАЙТ_№4 ] , ФЛАГ ] ); // Устанавливает светодиоды (сегменты) индикатора по битам.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMyMzU4NDIxMl19
-->