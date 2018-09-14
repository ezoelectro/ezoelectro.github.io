---
layout: post
title:  "Remdet5, переделка платы и корпуса"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: из-за Bluetooth 4.0 модуля
img: history06/V5_0_PCB01_SM.PNG # Add image post (optional)
---
<p>Разобрался я с Bluetooth 4.0 с использованием модуля BLE112, и не зря я не спешил заказывать платы. Модуль BLE112 по SPI не работает, чтото там с маленьким буфером. В общем он работает по RS-232, причем нужны линии RTS и CTS и дополнительные сигналы состояния. Изза этого переделал плату и корпус. В питание добавил LC фильтры, может пригодятся. Отработал спящие режимы BLE112. Данными могу обмениваться с компом и с iphone. Платы сегодня заказал. Версию устройства вернул к  5.0, полностью в живую такого еще не было. Платы придут тогда и корпус печатать буду. Может какието доработки нужно будет внести. Мне нужна толщина платы 0.5мм, но они почемуто получаются 0.6-0.7мм. Заказал 0.36мм, посмотрим какие они придут.</p>
<p><a  href="{{ site.baseurl }}/assets/images/history06/V5_0_CASE01.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history06/V5_0_CASE01_SM.JPG" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/history06/V5_0_CASE02.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history06/V5_0_CASE02_SM.JPG" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/history06/V5_0_PCB01.PNG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history06/V5_0_PCB01_SM.PNG" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/history06/V5_0_PCB02.PNG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history06/V5_0_PCB02_SM.PNG" alt="img" width="677" /></a></p>
<p><a  href="{{ site.baseurl }}/assets/images/history05/V5_0_SCH01.pdf">
   <img src="{{ site.baseurl }}/assets/images/history05/V5_0_SCH01.PNG" alt="img" width="677" /></a></p> 
