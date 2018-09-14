---
layout: post
title:  "Remdet4, фазы БДГ"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: Отфильтровка моментов когда двигается голова
img: history04/sleep_night_01_sm.jpg # Add image post (optional)
---
<p><br><a href="{{ site.baseurl }}/assets/images/history04/2sided_adhesive_tape.JPG" class="highslide" onclick="return hs.expand(this)">
      <img src="{{ site.baseurl }}/assets/images/history04/2sided_adhesive_tape_sm.JPG" alt="img" width="677" /></a></p>
<p>Приклеил на двусторонний скотч REMDETECTOR к маске, отлично держится,  вес вместе с маской 45грамм, маска отдельно 25грамм, REMDETECTOR отдельно 20гр. Прибор работал полностью автономно, все данные записывались во внутренюю память, т.е. никаких проводов в этот раз не было.  Была непривычность спать с маской, т.е. она ощущалась в пробуждениях. Но в целом спать прибор не мешал в отличии от предыдущих проводных версий. Аккамулятор за ночь сел примерно на 15%, так что возможно с энергоэкономией, а конкретно с использованием FERAM вместо FLASH я и перестарался, но посмотрим как BLUETOOTH версия будет хавать.В комп сливаю данные по USB СDC (виртуальный COM порт), USB HID пока не получается до конца сделать, под C++ Builder не могу данные в него читать и писать, но как устройство обнаруживается и имя производителя и название прибора могу и на C++ Builder прочитать. </p>
<p><img src="{{ site.baseurl }}/assets/images/history04/usb_hid_01.PNG" alt="img" width="677" class="img-rounded"></p> 
<p><img src="{{ site.baseurl }}/assets/images/history04/usb_hid_02.PNG" alt="img" width="677" class="img-rounded"></p> 
<p>Это эксперименты с HID под Windows, пока еще не доделал.</p>
<p><br>Далее разбор ночной записи с REMDETECTOR:</p>
<p><a href="{{ site.baseurl }}/assets/images/history04/sleep_night_01.png" class="highslide" onclick="return hs.expand(this)">
      <img src="{{ site.baseurl }}/assets/images/history04/sleep_night_01_sm.jpg" alt="img" width="677" /></a></p>
<p>Ночная запись, на красном графике движений глаз четко видно 3 зоны активных движений глаз. Период между ними примерно 1час 45 мин.</p>
<p>&nbsp;</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history04/sleep_night_02.png" class="highslide" onclick="return hs.expand(this)">
      <img src="{{ site.baseurl }}/assets/images/history04/sleep_night_02_sm.jpg" alt="img" width="677" /></a></p>
<p>Это первая фаза быстрых движений глаз в увеличенном масштабе, в конце ее видно микро пробуждение, а именно движение головы - синий график (акселерометр).</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history04/sleep_night_03.png" class="highslide" onclick="return hs.expand(this)">
      <img src="{{ site.baseurl }}/assets/images/history04/sleep_night_03_sm.jpg" alt="img" width="677" /></a></p>
<p>Вторая фаза быстрых движений глаз, уже видно два пробуждения с движением головы.</p>
<p>&nbsp;</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history04/sleep_night_04.png" class="highslide" onclick="return hs.expand(this)">
      <img src="{{ site.baseurl }}/assets/images/history04/sleep_night_04_sm.jpg" alt="img" width="677" /></a></p>
<p>Третья фаза быстрых движений глаз в увеличенном масштабе, пробуждений с движением головы уже значительно больше.</p>
<p><br><br>На следующих анимированных GIFах показанно, как работает фильтрация движений головы. Она удаляет из данных от глаза, те сегменты, где двигалась голова. Алгоритм простейший: при обнаружении от акселерометра уровня сигнала превосходящий заданный порог, игнорировать текущие данные от глаза и 19 последующих, всего 20, т.е. в сумме около 3 секунд.</p>
<p><img src="{{ site.baseurl }}/assets/images/history04/sleep_night_05.gif" alt="img" width="677" class="img-rounded"></p> 
<p>Вся ночь 8 часов 20мин</p>
<p><br><img src="{{ site.baseurl }}/assets/images/history04/sleep_night_06.gif" alt="img" width="677" class="img-rounded"></p> 
<p>Первая фаза 20мин</p>
<p><br><img src="{{ site.baseurl }}/assets/images/history04/sleep_night_07.gif" alt="img" width="677" class="img-rounded"></p> 
<p>Вторая фаза 20мин</p>
<p><br><img src="{{ site.baseurl }}/assets/images/history04/sleep_night_08.gif" alt="img" width="677" class="img-rounded"></p> 
<p>Третья Фаза 27мин</p>