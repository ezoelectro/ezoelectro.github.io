---
layout: post
title:  "Remdet"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: История разработки пробора
img: history07/glaz_animation01.gif # Add image post (optional)
---
<p>Первые тесты программого определения положения глаза. Четыре графика это данные с четырех фотодатчиков. На осоновании них движется анимация глаза. Это я пальцем вожу над датчиками:</p>
<p><img src="{{ site.baseurl }}/assets/images/history07/glaz_animation01.gif" alt="img"></p> 
<p><br>Вот инфракрасные датчики видно, 4 штуки, по центру яркий красный светодиод для вспышки:</p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_01.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_01_sm.JPG" alt="img" width="677" /></a></p>
<p><br>Не обошлось без косяков в схеме, на макетке я эту часть поленился потеститровать. В общем резистор должен быть возле каждого фототранзистора, иначе большие скачки у трех каналов получаются, либо нужно делать очень долгий опрос пока переходные процессы не устаканятся, а это замедляет быстродействие и батарейка быстрее съестся. В общем резюки нужны все четыре:</p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_02.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_02_sm.JPG" alt="img" width="677" /></a></p>
<p><br>Напаивал прям на плату:</p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_03.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_03_sm.JPG" alt="img" width="677" /></a></p>
<p><br>Корпус тоже пришлось подточить:</p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_04.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_04_sm.JPG" alt="img" width="677" /></a></p>
<p><br>Позже на плату поставлю вот такую сборку 0603 из четырех резисторов:</p>
<p><img src="{{ site.baseurl }}/assets/images/history07/YAGEO_array.jpg" alt="img" width="326" class="img-rounded"></p> 
<p><br>А так все выглядело после монтажа:</p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_05.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_05_sm.JPG" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/history07/remdet_V5_06.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history07/remdet_V5_06_sm.JPG" alt="img" width="677" /></a></p>
