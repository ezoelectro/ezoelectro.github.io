---
layout: post
title:  "Remdet5, принципиальная схема"
categories: Remdet
tags: Remdet
author: Alex Koblov
description: Переделка схемы
img: history05/V5_1_SCH02_sm.PNG # Add image post (optional)
---
<p>Уже буквально перед заказом печатных плат, выяснилось, что PIC18 микроконтроллеры J-серии в отличии от K-серии, не на всех портах могут держать 25мА, больше половины портов могут выдать только 4мА. В связи с этим переделал принципиальную схему и переразвел плату. Я от некоторых портов запитываю флэшку, акселерометр, усилитель, блютус модуль, инфракрасный светодиод в импульсном режиме с большим током.</p>
    
<p><a  href="{{ site.baseurl }}/assets/images/history05/V5_1_SCH02.pdf">
   <img src="{{ site.baseurl }}/assets/images/history05/V5_1_SCH02_sm.PNG" alt="img" width="677" /></a></p>
<p><br>Еще произошел казус, заказал на <a href="http://ru.aliexpress.com">Алиэкспрессе</a> микросхемы TS3A5017PW в корпусе TSSOP, а они пришли через 40 дней в корпусе TVSOP, деньги вернули, но пришлось заново перезаказать. Остальную комплектацию заказал в <a href="http://www.electronshik.ru">Электронщике</a>. TS3A5017PW в Электронщике тоже есть, но  там минимальная партия 55шт. Вообще интересно, как этот аналоговый ключь работает, ни разу его не пробовал.</p>
<p><a  href="{{ site.baseurl }}/assets/images/history05/TSSOP_TVSOP.JPG" class="highslide" onclick="return hs.expand(this)">
   <img src="{{ site.baseurl }}/assets/images/history05/TSSOP_TVSOP_sm.JPG" alt="img" width="677" /></a></p>