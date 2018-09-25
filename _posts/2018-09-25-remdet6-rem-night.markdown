---
layout: post
title:  "Remdet6, Ночная запись с видимыми REM фазами "
categories: Remdet
tags: Remdet
author: Alex Koblov
description: REM фазы с периодом примерно 1час40мин. Заметил нелинейность датчика VCNL3020
img: post002/pic1.png # Add image post (optional)
---
<p><br>Ночная запись:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post002/pic1.png" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post002/pic1.png" alt="img" width="677" /></a></p>
<p><br>Датчик VCNL3020 имеет видимую нелинейную зависимость расстояния и того значения что он выдает, нужно будет сделать линеаризацию. Тестовый стенд для измерения расстояния:</p>
<p><a  href="{{ site.baseurl }}/assets/images/post002/pic2.jpg" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/post002/pic2_sm.jpg" alt="img" width="677" /></a></p>
<a href="https://github.com/ezoelectro/ezoelectro.github.io/tree/master/REMDET_PROG/ble_test10(11)">Программа и ночная запись</a>
