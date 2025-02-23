---
title: "NEMA 23 i driveri"
header:
  teaser: /assets/img/posts/nema23_and_drivers.jpg
excerpt: "Za sve one kojima treba koračni (stepper) motor veće snage, u ponudu smo dodali NEMA 23 motor, kao i drivere koji mogu ukrotiti ovu zvijer - standardni DM524T, ali i *MKS-ov* driver baziran na **TMC 2160** čipu."
categories:
  - Mehatronika
tags:
  - NEMA
  - motor
  - driver
---

![nema 23 and drivers]({{ site.url }}{{ site.baseurl }}/assets/img/posts/nema23_and_drivers.jpg){: .align-center}

Za sve one kojima treba koračni (stepper) motor veće snage, u ponudu smo dodali *NEMA 23* motor, kao i drivere koji mogu ukrotiti ovu zvijer - standardni *DM524T*, ali i *MKS-ov* driver baziran na **TMC 2160** čipu.

{% capture fig_img %}
![nema 23 motor]({{ '/assets/img/posts/nema23.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>NEMA 23 koračni motor</figcaption>
</figure>

Prije godinu dana u ponudu smo dodali [NEMA 14 koračni motor](https://www.diykits.eu/products/p_12438) kao kompaktniju alternativu standardnim *NEMA 17* motorima kada nije potrebna tolika snaga, a prostor je skučen. Sada smo otišli u drugom smjeru i nabavili [NEMA 23](https://www.diykits.eu/products/p_12570) koja će dobro doći kada je potrebna veća snaga motora. Već sama masa motora od 1.6 kg dovoljan je pokazatelj što sve može - u konkretnim brojkama to je punih 3.0 Nm okretnog momenta i korak od 1.8°.

{% capture fig_img %}
![dm524t motor driver]({{ '/assets/img/posts/dm524t.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-right" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>DM524T digitalni stepper motor driver v4.0</figcaption>
</figure>

Za jaki motor, treba isto takav driver, a [DM524T](https://www.diykits.eu/products/p_12602) česti je izbor kada su u igri *NEMA 23* motori. Ima cijeli niz postavki koje je moguće podesiti, od toga hoće li logika raditi na 5 ili 24 V, pa do 16 različitih postavki za mikrokorake. Napajanje može biti u rasponu od 18~50 VDC, maksimalna vršna struja 4.5 A, ima podršku za PUL/DIR način rada, zaštitu od prenapona i prekomjerne struje.

{% capture fig_img %}
![tmc 2160 motor driver]({{ '/assets/img/posts/tmc2160-oc.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>MKS TMC2160-OC v1.0 stepper motor driver</figcaption>
</figure>

Iako moćan, *DM524T* driver prilično je glomazan, pa smo nabavili i kompaktniju alternativu, ovaj put baziranu na *Trinamicovom* **TMC 2160** čipu. Iako ima malo manje opcija, [ovaj driver](https://www.diykits.eu/products/p_12584) nudi mogućnost korištenja naprednih tehnologija kao što su *spreadCycle* i *stealthChop*. Tu je i optička izolacija ulaznog signala (radi s 5V logikom), a podržana su napajanja u rasponu od 8-40 V DC. Treba pripaziti na to da je minimalna jakost struje 2.3 A, što će za neke manje motore biti previše.