---


---

<p><a href="https://iarduino.ru"><img src="https://iarduino.ru/img/logo.svg" alt=""></a><a href="https://iarduino.ru"><img src="https://wiki.iarduino.ru/img/git-shop.svg?3" alt=""></a> <a href="https://wiki.iarduino.ru"><img src="https://wiki.iarduino.ru/img/git-wiki.svg?2" alt=""></a> <a href="https://lesson.iarduino.ru"><img src="https://wiki.iarduino.ru/img/git-lesson.svg?2" alt=""></a><a href="http://forum.trema.ru"><img src="https://wiki.iarduino.ru/img/git-forum.svg?2" alt=""></a></p>
<h1 id="iarduino_pressure_bmp-скачать">iarduino_Pressure_BMP <a href="https://github.com/tremaru/iarduino_Pressure_BMP/archive/master.zip">СКАЧАТЬ</a></h1>
<p>Библиотека iarduino_Pressure_BMP позволяет считывать температуру окружающей среды и атмосферное давление с датчиков <a href="http://iarduino.ru/shop/Sensory-Datchiki/barometr-gy-68-datchik-atmosfernogo-davleniya-bmp180.html">BMP180</a> и <a href="http://iarduino.ru/shop/Sensory-Datchiki/barometr-trema-modul.html">BMP280</a>, а так же рассчитывать высоту.</p>
<blockquote>
<p>Подробнее про установку библиотеки читайте в нашей <a href="https://wiki.iarduino.ru/page/Installing_libraries/">инструкции</a>.</p>
</blockquote>
<p>Пример подключения к <a href="https://iarduino.ru/shop/boards/arduino-uno-r3.html">Arduino</a>/<a href="https://iarduino.ru/shop/boards/piranha-uno-r3.html">Piranha UNO</a> с помощью <a href="https://iarduino.ru/shop/Expansion-payments/trema-shield.html">Trema Shield</a></p>
<p>Подробнее о <a href="https://wiki.iarduino.ru/page/trema-modul-pressure-meter">подключении модуля</a></p>
<p><img src="https://iarduino.ru/img/upload/ff71929a63d941fd58dc5a60860d0671.png" alt="enter image description here"></p>
<p>| Модель | Ссылка на магазин|</p>
<p>|–|--|</p>
<p>| BMP280 <img src="https://wiki.iarduino.ru/img/resources/840/840.svg" alt="enter image description here"> | <a href="https://iarduino.ru/shop/Sensory-Datchiki/barometr-trema-modul.html%7C">https://iarduino.ru/shop/Sensory-Datchiki/barometr-trema-modul.html|</a></p>
<p>| BMP180 <img src="https://wiki.iarduino.ru/img/resources/840/840.svg" alt="enter image description here"> | <a href="https://iarduino.ru/shop/Sensory-Datchiki/barometr-gy-68-datchik-atmosfernogo-davleniya-bmp180.html">https://iarduino.ru/shop/Sensory-Datchiki/barometr-gy-68-datchik-atmosfernogo-davleniya-bmp180.html</a> |</p>
<h2 id="описание-библиотеки">Описание библиотеки:</h2>
<p>Данная библиотека может использовать как аппаратную, так и программную реализацию шины I2C.</p>
<p>О том как выбрать тип шины I2C рассказано в статье <a href="https://wiki.iarduino.ru/page/i2c_connection/">Wiki - расширенные возможности библиотек iarduino для шины I2C</a>.</p>
<p><strong><a href="https://wiki.iarduino.ru/page/trema-modul-pressure-meter"> Подробное описание, подключение и примеры работы </a></strong></p>
<h2 id="назначение-функций-и-переменных">Назначение функций и переменных:</h2>
<p>Подробное описание работы с библиотекой, находится в разделе <a href="https://wiki.iarduino.ru/page/chetyrehrazryadnyy-indikator-trema-modul/" title="Wiki Четырёхразрядный индикатор">Wiki Четырёхразрядный индикатор</a>.</p>
<p><strong>Подключаем библиотеку.</strong></p>
<p>#include <strong>&lt;iarduino_Pressure_BMP.h&gt;</strong> // Подключаем библиотеку.</p>
<p><strong>Создаём объект (адрес по умолчанию 0x77).</strong></p>
<p>iarduino_Pressure_BMP <strong>ОБЪЕКТ (</strong> [ АДРЕС_I2C ] <strong>);</strong> // Создаём объект (адрес по умолчанию 0x77).</p>
<p><strong>Инициализация работы BMP датчика (с указанием его начальной высоты).</strong></p>
<p>Функция <strong>begin(</strong> [ ВЫСОТА ] <strong>);</strong> // Инициализация работы BMP датчика (с указанием его начальной высоты).</p>
<p><strong>Чтение показаний датчика (с выбором единицы измерения давления).</strong></p>
<p>Функция <strong>read(</strong> [ ЦИФРА ] <strong>);</strong> // Чтение показаний датчика (с выбором единицы измерения давления).</p>
<p><strong>Выбор точности измерений (подавление шума).</strong></p>
<p>Функция <strong>measurement(</strong> ЦИФРА <strong>);</strong> // Выбор точности измерений (подавление шума).</p>
<p><strong>Возвращает температуру окружающей среды в °С.</strong></p>
<p>Переменная <strong>temperature</strong> // Возвращает температуру окружающей среды в °С.</p>
<p><strong>Возвращает атмосферное давление в мм.рт.ст. или Па.</strong></p>
<p>Переменная <strong>pressure</strong> // Возвращает атмосферное давление в мм.рт.ст. или Па.</p>
<p><strong>Возвращает высоту относительно начальной в м.</strong></p>
<p>Переменная <strong>altitude</strong> // Возвращает высоту относительно начальной в м.</p>
<p><strong>Возвращает тип датчика: 180 или 280.</strong></p>
<p>Переменная <strong>type</strong> // Возвращает тип датчика: 180 или 280.</p>
<p><strong>Возвращает версию прошивки датчика.</strong></p>
<p>Переменная <strong>version</strong> // Возвращает версию прошивки датчика.</p>
<!--stackedit_data:&#10;&#10;eyJoaXN0b3J5IjpbLTEzNjk3NzY1MDldfQ==&#10;&#10;-->

