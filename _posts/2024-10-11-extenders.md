---
title: "Ekspanderi, ekstenderi, multiplekseri"
header:
  teaser: /assets/img/posts/extenders.jpg
excerpt: "Česta je pojava da se u projekt u hodu dodaju senzori, aktuatori i druge komponente i onda odjednom ponestane priključaka. Tu u spas dolaze razni ekstenderi, ekspanderi i multiplekseri"
categories:
  - Elektronika
tags:
  - Adafruit
---

![arduino mega with many connections]({{ site.url }}{{ site.baseurl }}/assets/img/posts/extenders.jpg){: .align-center}

Česta je pojava da se u projekt u hodu dodaju senzori, aktuatori i druge komponente i onda odjednom ponestane priključaka. Tu u spas dolaze razni ekstenderi, ekspanderi i multiplekseri, a mi smo iz *Adafruita* upravo dobili tri različita i jako zanimljiva uređaja baš iz te kategorije. Pa krenimo redom.

{% capture fig_img %}
![attiny1616 seesaw]({{ '/assets/img/posts/attiny-seesaw.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Adafruit ATtiny1616 seesaw</figcaption>
</figure>

[Ova pločica](https://www.diykits.eu/products/p_12647) bazirana je na *ATtiny1616* mikrokontroleru i teoretski bi mogla biti samostalna mikrokontrolerska pločica, ali zahvaljujući unaprijed instaliranom Adafruitovom **seesaw** *firmwareu* ponaša se kao *I2C na svašta/nešto* konverter. Ovo omogućava jednostavno proširenje bilo kojeg projekta s 12x GPIO, 9x 10-bit ADC, 5x 8-bit PWM, 1x NeoPixel izlazom, 1x interrupt, 1x LED i 127 byte EEPROM-a. Radi s 2-5 V napajanjem/logikom pa pokriva sve *Arduino/Raspberry/ESP* projekte, a može se jednostavno povezati s mikrokontrolerskom pločicom putem StemmaQT/Qwiic/EasyC I<sup>2</sup>C konektora.

{% capture fig_img %}
![PCA9546 multiplexer]({{ '/assets/img/posts/PCA9546-multiplexer.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-right" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Adafruit PCA9546 multiplekser</figcaption>
</figure>

Ova pločica rješenje je malo drugačijeg problema: korištenje nekoliko istih I<sup>2</sup>C periferija koje imaju identičnu (i nepromjenjivu) adresu pa ne mogu biti na istom I<sup>2</sup>C busu. Uz pomoć ovog [multipleksera](https://www.diykits.eu/products/p_12648) možete povezati do četiri periferije s identičnim I<sup>2</sup>C adresama korištenjem *StemmaQT/Qwiic/EasyC* konektora za brzo i jednostavno povezivanje. Napajanje/logika je u rasponu 3-5 V uz podržani level shifting 5->3.3 V (korištenjem jumpera) na izlaznim konektorima. Adresa uređaja je 0x70, moguće je promijeniti u rasponu od 0x70-0x77, tj. koristiti 8 ovih uređaja istovremeno, što daje ukupno 32 uređaja s istom I<sup>2</sup>C adresom!

{% capture fig_img %}
![TCA8418 tipkovnički driver]({{ '/assets/img/posts/keyboard-matrix-expander.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0; width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Adafruit TCA8418 tipkovnički driver i GPIO ekspander</figcaption>
</figure>

Ako nešto zauzima puno I/O pinova, onda su to razne tipkovnice, npr. matrica 4x4 otet će 8 pinova, a nije da je nešto posebno velika. Tu na scenu stupa [Adafruit TCA8418 tipkovnički driver](https://www.diykits.eu/products/p_12649) koji ima ukupno 18 I/O pinova, 10 stupaca i 8 redaka koji pokrivaju tipkovničke matrice do ukupno 80 tipaka, ali se mogu koristiti i kao uobičajeni GPIO pinovi. Ako priključite tipkovnicu, driver će voditi brigu o pritisku na tipke, uključujući i FIFO queue od 10 elemenata. Pločica se povezuje preko I<sup>2</sup>C (kompatibilna je s StemmaQT/Qwiic/EasyC), postoje Arduino i CircuitPython biblioteke, kao i Linux kernel driver pa se može koristiti i direktno na Raspberry Pi-u.
