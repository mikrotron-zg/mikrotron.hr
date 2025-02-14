---
title: "Srcotron"
excerpt: "Kućni EKG kit baziran na Arduinu."
header:
  teaser: assets/img/srcotron_kit.jpg
developed_by: Josip Almaši, Tomislav Mamić
last_modified_at: 2016-11-06T20:00:00+01:00
---

![image-center]({{ site.url }}{{ site.baseurl }}/assets/img/srcotron_kit.jpg){: .align-center}

Srcotron omogućuje mjerenje EKG signala pomoću Olimex EKG-EMG shielda i Arduino UNO platforme. Ovo je najjeftinije moguće rješenje za mjerenje i snimanje EKG signala u kućnoj radinosti. Napisali smo i *Python* skriptu koja će na računalu napraviti vizualizaciju signala, baš kao pravi EKG uređaj! Kompletni kod ovog rješenja objavljen je kao open source na [githubu](https://github.com/mikrotron-zg/srcotron).

{% capture fig_img %}
![image-center]({{ '/assets/img/srcotron.png' | relative_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Screenshot vizualizacije na računalu</figcaption>
</figure>

Kit se sastoji od:
* mikrokontrolerske pločice Iteaduino UNO (bilo koja Arduino UNO kompatibilna pločica će raditi)
* EKG štita (shielda) Olimex Shield-EKG-EMG
* elektroda Olimex Shield-EKG-EMG-PA
* 3D printane kutije i 3 vijka M3x8
* USB kabela tip A - mini B (ili neki drugi koji odgovara Arduino UNO pločici)
