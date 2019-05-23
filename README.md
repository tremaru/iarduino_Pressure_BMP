---


---

<p>https://iarduino.ru"><img src="  

[![](https://iarduino.ru/img/logo.svg" alt=""></a><a href=")](https://iarduino.ru"><img src=")[![](https://wiki.iarduino.ru/img/git-shop.svg?3" alt=""></a> <a href=")](https://wiki.iarduino.ru"><img src=") [![](https://wiki.iarduino.ru/img/git-wiki.svg?2" alt=""></a> <a href=")](https://lessonwiki.iarduino.ru"><img src=") [![](https://wiki.iarduino.ru/img/git-lesson.svg?2" alt=""></a><a href=")](https://forum.trema.ru"><img src="lesson.iarduino.ru)[![](https://wiki.iarduino.ru/img/git-forum.svg?2" alt=""></a></p>
<h1 id="iarduino_pressure_bmp-скачать">)](http://forum.trema.ru)

  

# iarduino_Pressure_BMP <a href="[СКАЧАТЬ](https://github.com/tremaru/iarduino_Pressure_BMP/archive/master.zip">СКАЧАТЬ</a></h1>
<p>)

Библиотека iarduino_Pressure_BMP позволяет считывать температуру окружающей среды и атмосферное давление с датчиков <a href="[BMP180](http://iarduino.ru/shop/Sensory-Datchiki/barometr-gy-68-datchik-atmosfernogo-davleniya-bmp180.htmlBMP1280<8p://iarduino.ru/shop/Sensory-Datchiki/barometr-trema-modul.html, а так же рассчитывать высоту.

  

> Подробнее про установку библиотеки читайте в нашей <a href="[инструкции](https://iarduino.ru/page/Installing_libraries/).

  

Пример подключения к [Arduino](https://iarduino.ru/shop/boards/arduino-uno-r3.html)/[Piranha UNO](https://iarduino.ru/shop/boards/piranha-uno-r3.html) с помощью [Trema Shield](https://iarduino.ru/shop/Expansion-payments/trema-shield.html)

Подробнее о [подключении модуля](https://wiki.iarduino.ru/page/trema-modul-pressure-meter)

![enter image description here](https://iarduino.ru/img/upload/ff71929a63d941fd58dc5a60860d0671.pngenter image description here"></p>
<p>| Модель | Ссылка на магазин|</p>
<p>|–|--|</p>
<p>| BMP280 <img src="https://wiki.iarduino.ru/ |

  

## Описание библиотеки:Данная библиотека может использовать как аппаратную, так и программную реализацию шины I2C.</p>
<p>

О том как выбрать тип шины I2C рассказано в статье Wiki - расширенные возможности библиотек iarduino для шины I2Chttps://wiki.iarduino.ru/page/i2c_connection/).

  

**[ Подробное описание, подключение и примеры работы Назначение функций и переменных:Подробное описание работы с библиотекой, находится в разделе [Wiki Четырёхразрядный индикатор](https://wiki.iarduino.ru/page/chetyrehrazryadnyy-indikator-trema-modul/"Wiki Четырёхразрядный индикатор">Wiki Четырёхразрядный индикаg>Подключаем библиотеку. <strong>&lt;).

  

**Подключаем библиотеку.**

  

#include **<iarduino_Pressure_BMP.h</strong>>** // Подключаем библиотеку.*Создаём объект (адрес по умолчанию 0x77).iarduino_Pressure_BMP>**

  

iarduino_Pressure_BMP <strong>ОБЪЕКТ (</strong> [ АДРЕС_I2C ] <strong>);</strong>**ОБЪЕКТ (** [ АДРЕС_I2C ] **);** // Создаём объект (адрес по умолчанию 0x77).Инициализация работы BMP датчика (с указанием его начальной высоты).</strong></p>
<p>Функция <strong>begin(</strong> [ ВЫСОТА ] <strong>);</strong>**

  

Функция **begin(** [ ВЫСОТА ] **);** // Инициализация работы BMP датчика (с указанием его начальной высоты).*Чтение показаний датчика (с выбором единицы измерения давления).</strong></p>
<p>Функция <strong>read(</strong> [ ЦИФРА ] <strong>);</strong>**

  

Функция **read(** [ ЦИФРА ] **);** // Чтение показаний датчика (с выбором единицы измерения давления).</p>
<p><strong>

  

**Выбор точности измерений (подавление шума).</strong></p>
<p>Функция <strong>measurement(</strong> ЦИФРА <strong>);</strong>**

  

Функция **measurement(** ЦИФРА **);** // Выбор точности измерений (подавление шума).</p>
<p><strong>

  

**Возвращает температуру окружающей среды в °С.>**

  

Переменная <strong>**temperature</strong>** // Возвращает температуру окружающей среды в °С.g>

  

**Возвращает атмосферное давление в мм.рт.ст. или Па.>Переменная <strong>pressure</strong>**

   // Возвращает атмосферное давление в мм.рт.ст. или Па.</p>
<p><strong>

  

**Возвращает высоту относительно начальной в м.</strong></p>
<pПеременная <strong>altitude</strong>**

  // Возвращает высоту относительно начальной в м.</p>
<p><strong>

  

**Возвращает тип датчика: 180 или 280.>Переменная <strong>type</strong>**
 // Возвращает тип датчика: 180 или 280.*Возвращает версию прошивки датчика.</strong></p>
<p>Переменная <strong>version</strong // Возвращает версию прошивки датчика.</p>

  
  
  
  
  
  
  
  
  
  

<!--stackedit_data:&#10;&#10;

eyJoaXN0b3J5IjpbLTEzNjk3NzY1MDldfQ==&#10;&#10;

-->

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4Mzk3NjMxMzVdfQ==
-->