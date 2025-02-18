---
title: "Slidertron"
excerpt: "Slider za kameru/fotoaparat kojim se upravlja preko WiFi-a."
header:
  teaser: assets/img/slidertron.jpg
developed_by: Tomislav Preksavec
last_modified_at: 2022-06-10T20:00:00+01:00
---

![image-center]({{ site.url }}{{ site.baseurl }}/assets/img/slidertron.jpg){: .align-center}

ESP32 pretvorio se u našu najdražu osnovu za elektroničke i mehatroničke projekte, a ovo je školski primjer zašto je tome tako. Ideja uređaja koji pomiče kameru ili fotoaparat lijevo-desno nije ništa novo, ali iznenadilo bi vas koliko malo ih ima na tržištu koji nude bežično upravljanje, a da ne koštaju pravo malo bogatstvo. Iskoristili smo mogućnost ESP32 mikrokontrolera da bude minijaturni web server pa se za upravljanje uređajem može koristiti bilo koji WiFi uređaj (npr. smartphone ili laptop). Ako se u miks ubaci i websocket protokol, onda je odaziv uređaja praktički trenutni, bez obzira radi li se o relativno brzom pomicanju kamere ili o ultrasporom timelapseu fotoaparata.

![image-center]({{ site.url }}{{ site.baseurl }}/assets/img/slidertron_box.jpg){: .align-center}

Ovaj mali projekt bio je platforma za nekoliko konkretnih poslova i zaslužio je svoj open source [github repozitorij](https://github.com/mikrotron-zg/slidertron). 