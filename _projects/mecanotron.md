---
title: "Mecanotron"
excerpt: "Robotski automobil s mecanum (omnidirekcijskim) kotačima."
header:
  teaser: assets/img/mecanotron.jpg
developed_by: Tomislav Preksavec
last_modified_at: 2024-09-27T20:00:00+01:00
---

![image-center]({{ site.url }}{{ site.baseurl }}/assets/img/mecanotron.jpg){: .align-center}

Za razliku od naših [Autotron autića]({{ site.url }}{{ site.baseurl }}/projects/autotron), ovaj je specifičan po omnidirekcijskim (tzv. *mecanum*) kotačima koje koristi, a koji mu omogućuju načine kretanja koji se inače ne mogu postići korištenjem klasičnih kotača. Tako se on može okrenuti na mjestu i kretati postrance ili po dijagonali - sve skupa ima 18 različitih načina kretanja! Video sa svim mogućim načinima kretanja možete pogledati na našem
[TikTok kanalu](https://www.tiktok.com/@mikrotron/video/7193331245403671813?is_from_webapp=1&sender_device=pc&web_id=7467939093768226326).

![image-left]({{ site.url }}{{ site.baseurl }}/assets/img/mecanotron_control.jpg){: .align-left}

Najveći je izazov bio isprogramirati sve ove načine kretanja, tako da smo na kraju napravili cijeli library za ovaj pogon, možete ga naći u sklopu [github repozitorija](https://github.com/mikrotron-zg/mecanotron) ovog projekta. Isto tako, bilo je zabavno napraviti korisničko sučelje za upravljanje vozilom, ali pošto smo ponovno koristili mogućnost ESP32 mikrokontrolera da bude web server, web aplikacija s puno gumbića riješila je i taj problem.