---
layout: post
title:  "Remdet4, цифровые фильтры"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: Программа для тестирования разных фильтров
img: history03/filtr_test_4.PNG # Add image post (optional)
---
<p>Тестирование цифровых фильтров:</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_1.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_1.PNG" alt="img" width="600" /></a></p>
<p>Исходный сигнал</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_2.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_2.PNG" alt="img" width="600" /></a></p>
  <p>Фильтр 2 порядка 5Гц</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_3.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_3.PNG" alt="img" width="600" /></a></p>
  <p>Добавлен фильтр 2 порядка 0.19Гц</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_4.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_4.PNG" alt="img" width="600" /></a></p>
  <p>Серым цветом показан  полосовой фильтр 2 порядка 0.19-5Гц примененный к исходному сигналу. Видно что разница не значительна. Поэтому нет смысла использовать последовательно два фильтра. Можно сразу этот полосовой.</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_5.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_5.PNG" alt="img" width="600" /></a></p>
<p><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_6.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_6.PNG" alt="img" width="600" /></a></p>
  <p>ABS() сигнала, т.е. все отрицательное стало положительным.</p>
<p><br><a href="{{ site.baseurl }}/assets/images/history03/filtr_test_7.PNG" class="highslide" onclick="return hs.expand(this)">
  <img src="{{ site.baseurl }}/assets/images/history03/filtr_test_7.PNG" alt="img" width="600" /></a></p>
  <p>Полученный сигнал. Далее у него понижается частота дескритизации, и разрядность. О чем писалось выше.</p>