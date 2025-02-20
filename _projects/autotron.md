---
title: "Autotron"
excerpt: "Nekoliko projekata kojima je zajednički nazivnik maleni robotski autić."
header:
  teaser: assets/img/autotron.jpg
developed_by: Tomislav Mamić, Tomislav Preksavec
last_modified_at: 2018-04-05T20:00:00+01:00
---



{% capture fig_img %}
![image-center]({{ '/assets/img/autotron.jpg' | absolute_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Autotron Basic</figcaption>
</figure>

U svojoj prvoj inkarnaciji, **Autotron Basic** bio je baziran na *Arduino UNO-u* u kombinaciji s njihovim *Motor Shieldom* i ultrazvučnim daljinomjerom. Znao se samostalno kretati po prostoriji i izbjegavati prepreke, ali to je bio vrhunac njegovih mogućnosti.

{% capture fig_img %}
![image-center]({{ '/assets/img/autotron_nova.jpg' | absolute_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Autotron Nova</figcaption>
</figure>

Negdje u to doba, ekipa iz tadašnje *e-radionice* (danas [soldered.com](https://soldered.com/hr/)) izbacila je na tržište *Croduino Novu* baziranu na ESP8266 čipu pa smo morali isprobati može li naš Autotron postati autić na WiFi daljinsko upravljanje. Tako je nastao **Autotron Nova**, ovaj put isključivo ovisan o ljudskom upravljanju (mda, nije baš neki napredak <i class="fa-regular fa-face-smile-wink"></i>). Oba ova projekta, kao i eksperiment koji je koristio *MBoard* ITEAD Studia, možete pronaći na [githubu](https://github.com/mikrotron-zg/autotron).

{% capture fig_img %}
![image-center]({{ '/assets/img/autotron_pi.jpg' | absolute_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Autotron Pi</figcaption>
</figure>

Nakon *Arduino/ESP* platforme, došlo je vrijeme da naš autić opremimo nečim malo jačim, pa je iduća verzija dobila *Raspberry Pi 3* pod haubu i novo originalno ime, **Autotron Pi**. Ovo nam je omogućilo da dodamo i kameru pa je sada daljinsko upravljanje postalo stvarno *daljinsko* - mogli ste njime upravljati i s druge strane svijeta (ofkors, ako imate pristup internetu). Projekt je zaslužio i svoju stranicu na [hackaday.io](https://hackaday.io/project/17929-autotron-pi) gdje možete pronaći sve detalje o ovoj verziji Autotrona.

{% capture fig_img %}
![image-center]({{ '/assets/img/autotron_zero.jpg' | absolute_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Autotron Pi Zero</figcaption>
</figure>

Zadnja inkarnacija ovog autića koristi *Raspberry Pi Zero (2)W* kao osnovu, u kombinaciji s širokokutnom kamerom radi bolje preglednosti. Ime je naravno **Autotron Pi Zero**, funkcionalnost je ostala ista kao i kod starijeg brata, a detalji su opet na [hackaday.io stranici](https://hackaday.io/project/94433-autotron-pi-zero). Obje RPi verzije imaju zajednički [github repozitorij](https://github.com/mikrotron-zg/autotron-pi).