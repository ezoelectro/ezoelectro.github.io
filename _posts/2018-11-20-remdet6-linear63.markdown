---
layout: post
title:  "Remdet6, Линеаризация по 63м точкам"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: Калибровка датчика VCNL3020
img: post006/linear63points.png # Add image post (optional)
---
<p><br>Сделал линеаризацию по 63 точкам, хотя изначально было 127:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post006/linear63points.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post006/linear63points.png" alt="img" width="677" /></a></p>
<p><br>Калибровку делал по бежевому цвету, намазал тональным кремом прикленный малярный скотч:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post006/linear63points6.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post006/linear63points6_sm.jpg" alt="img" width="677" /></a></p>
<p><br>Одел маску и записал график с разными ее положениями на лице, с придавленной максимально близко к глазу, как будто подушкой придавило, и влево и вправо смещал и вверх и вниз и придавливал и отпускал, в общем во всевозможных положениях, и применил к нему линеаризацию:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post006/linear63points2.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post006/linear63points2.png" alt="img" width="677" /></a></p>
<p><br>А здесь применил линеаризацию к старому ночному графику:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post006/linear63points3.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post006/linear63points3.png" alt="img" width="677" /></a></p>
<p><br>Здесь видно почему я отказался от линеаризации на 127 точек. Скорее всего шаги двигателя не идеально равные между собой, четные и 
не четные, не равны между собой. Может это глюк контроллера, может обмоток двигателя или механики червячной передачи, может программы, хотя все перепроверил много раз.  Я пробовал и 1/2 шага 
и 1/4 и 1/8, увеличивая соответственно количество маленьких шагов до 2,4,8, все равно они не равные были. Т.е. например первые 8 шагов 1/8 режима, не были равны вторым 8ми шагам,
 а вот третьим равны, четвертым опять не равны. Забил на этот глюк. Здесь использовался полный шаг. Вообще 127 шагов это максимальное расстояние для полного шага, дальше каретке просто некуда ехать, 
 да и расстояние уже почти 20мм от датчика(до глаза), врядли больше нужно. Можно перейти на режим 1/2 шага, снять тогда 256 шагов, и проредить до 128. Но думаю пока и 63 хватит:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post006/linear63points4.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post006/linear63points4.png" alt="img" width="677" /></a></p>
<p><br>Всего двигатель сделал 127 шагов, после каждого он замирал, чтобы все успокоилось (зеленый график), записывалась калибровочная точка. Далее по COM-порту(FT232R USB<->UART), шла комманда сделать следующий шаг:</p>
<p><img src="{{ site.baseurl }}/assets/images/post006/linear63points5.gif" alt="img" width="677"></p>
