---
title: "Nove igračke iz Adafruita"
header:
  teaser: /assets/img/posts/qtpy-risc-v.jpg
excerpt: "Za kraj godine (taman pred Božić) stigle su nam nove igračke iz Adafruitove kuhinje. Svakako treba izdvojiti *QT Py CH32V203* baziran na RISC-V arhitekturi, drugi u našoj ponudi nakon"
categories:
  - Elektronika
tags:
  - Adafruit
  - RISC-V
  - pohrana podataka
---

![qtpy risc-v]({{ site.url }}{{ site.baseurl }}/assets/img/posts/qtpy-risc-v.jpg){: .align-center}

Za kraj godine (taman pred Božić) stigle su nam nove igračke iz Adafruitove kuhinje. Svakako treba izdvojiti *QT Py CH32V203* baziran na RISC-V arhitekturi, drugi u našoj ponudi nakon [ESP32-C3-MINI pločice](https://www.diykits.eu/products/p_12515).

{% capture fig_img %}
![qtpy CH32V203G6]({{ '/assets/img/posts/qtpy-risc-v-front.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>QT Py CH32V203G6</figcaption>
</figure>

U standardnom *QT Py / XIAO formatu* CH32V203G6 ima jednu 32-bit RISC-V jezgru na 144 MHz, 10 KB SRAM-a i 32 KB flash memorije. Tu su i ostale očekivane điđe: ADC, timeri, native USB, UART, I2C (s EasyC/Qwiic/Stemma QT konektorom) i SPI. Ono čega nema je podrška za Circuit ili Micro Python, a i Arduino podrška za sada je u razvoju - ovo nije pločica za početnike, ali definitivno ćemo viđati sve više RISC-V mikrokontrolera pa je ovo dobra prilika za isprobati njihove mogućnosti. Na pločicu je taman stao i čuveni *EasyC/Qwiic/StemmaQT* konektor, pa je spajanje I<sup>2</sup>C periferije super jednostavno.

{% capture fig_img %}
![WCH CH9102F Friend]({{ '/assets/img/posts/ch9102f-friend.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-right" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>WCH CH9102F Friend</figcaption>
</figure>

Još jedna promjena u čipu koji se koristi dolazi iz kategorije *USB/UART konvertera*, to je [Adafruit WCH CH9102F Friend](https://www.diykits.eu/products/p_12676), a stiže i na druge *Adafruitove* proizvode kao zamjena za FTR232, FT231x ili CP210x čipove. Trenutno ovo zahtjeva instalaciju novih drivera na Windows i Mac OS operativnim sustavima, što se Linuxa tiče podrška je u kernelu, pa sve radi automagično. Kao i obično kod Adafruita, headeri su priloženi, ali nisu zalemljeni, pa ćete morati zagrijati lemilicu i prionuti na posao prije prve upotrebe.

{% capture fig_img %}
![qspi flash breakout]({{ '/assets/img/posts/qspi-flash.jpg' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>QSPI Flash pločica - 128 MBit 16 MB</figcaption>
</figure>

Za kraj jedna minijaturna pločica koja je zapravo samo razvod za Flash čip koji na njoj obitava. [Adafruit QSPI Flash pločica](https://www.diykits.eu/products/p_12677) najjednostavniji je način za dodavanje 16 MB Flash memorije koja će s mikrokontrolerom komunicrati preko brzog QSPI sučelja. Kad u projektu ponestane memorije, spas stiže u ovom malenom formatu - teško je reći, ali sa svojih 11.2x10.2x3.5 mm, vjerojatno je ovo najmanja pločica koju imamo u ponudi.