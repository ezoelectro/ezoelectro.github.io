---
layout: post
title:  "Remdet6, Нелинейность датчика"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: Наглядный вид нелинейности датчика VCNL3020
img: post004/pic4_sm.png # Add image post (optional)
---
<p><br>Купил старый DVD привод за 100руб(1.5$), разобрал, и на его базе сделал более точный стенд для калибровки нелинейности:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic1.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic1_sm.jpg" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic2.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic2_sm.jpg" alt="img" width="677" /></a></p>
<p><br>Драйвер шагового двигателя A4988 использовал готовый покупной(150руб), только отрегулировал силу тока подстроечным резистором, чтобы моторчик не грелся и шаги не пропускал.</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic3.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic3_sm.jpg" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic5.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic5_sm.jpg" alt="img" width="677" /></a></p>
<p><br>Моторчик может двигаться на заданное количество шагов в одну и другую сторону, с разной заданной скоростью. Вот какой график в итоге получился:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic4.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic4_sm.png" alt="img" width="677" /></a></p>
<p><br>Видно, что на графике расстояние Y1 не равно расстоянию Y5, а должно. Потомучто в реальности и там и там моторчик двигался на 5 шагов. Смысл линеаризации - применить к этому графику такой алгоритм, чтобы он выравнял расстояния Y1,Y2,Y3,Y4,Y5 между собой, так же A1-A5 между собой.</p>
<p><img src="{{ site.baseurl }}/assets/images/post004/test_stend2.gif" alt="img" width="677"></p> 
<p><br>Серый, белый, и черный цвета светоотражающей поверхности:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic01.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic01_sm.jpg" alt="img" width="677" /></a></p>
<p><br>График так же меняется от светоотражающей способности поверхности:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic02.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic02_sm.png" alt="img" width="677" /></a></p>
<p><br>Так движется тестовый стенд, скорость видео увеличена в 4 раза:</p>
<p><img src="{{ site.baseurl }}/assets/images/post004/stend2_move.gif" alt="img" width="400"></p>
<p><br>Графики с увеличением:</p>
<p><img src="{{ site.baseurl }}/assets/images/post004/gray_white_black_gray.gif" alt="img" width="677"></p>
<p><br>Видно что после применения Hi-Pass фильтра, который пропускает все что выше 2Гц, различия в значении амплитуд достаточно большие, поэтому нужна линеаризация:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic03.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic03_sm.png" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/post004/pic04.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post004/pic04_sm.png" alt="img" width="677" /></a></p>
 
