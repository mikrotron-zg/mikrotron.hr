---
title: "Izvori znanja"
header:
  teaser: /assets/img/posts/izvori-znanja-header.jpg
excerpt: "Iako je internet (pre)bogat raznim resursima, neki put je teško pronaći one kvalitetne jer ih često kvantiteta sakrije. Zato donosimo kratki popis izvora znanja koje i sami često koristimo."
categories:
  - Ostalo
tags:
  - Adafruit
  - Arduino
  - ESP32
  - Raspberry Pi
---

![izvori znanja grafika]({{ site.url }}{{ site.baseurl }}/assets/img/posts/izvori-znanja-header.jpg){: .align-center}

Iako je internet (pre)bogat raznim resursima, neki put je teško pronaći one kvalitetne jer ih često kvantiteta sakrije. Zato donosimo kratki popis izvora znanja koje i sami često koristimo.

{% capture fig_img %}
![adafruit logo]({{ '/assets/img/posts/adafruit_logo.png' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
</figure>

Odmah na početku krećemo s jednom od najbogatijih i najkvalitetnijih baza znanja kada su u pitanju Arduino bazirani mikrokontroleri i senzori - [Adafruit Learning System](https://learn.adafruit.com/). Ne samo što ćete ovdje pronaći vrlo detaljne upute, kako hardverske, tako i softverske, nego će te upute vrijediti bez obzira na to što ne koristite originalne [Adafruit](https://www.adafruit.com/) proizvode. Naime, Adafruit proizvodi su open source/hardware pa će velika većina proizvoda koje nabavite iz drugih izvora biti neki od klonova, što znači da će biti 100% kompatibilni s [Adafruitovim bibliotekama](https://github.com/adafruit) (koje su _de facto_ industrijski standard), a najčešće su i hardverski identični (o kvaliteti ovaj put nećemo). Također, u softverskom dijelu nije pokriven samo C/C++ kod, nego i [CircuitPython](https://circuitpython.org/) (njihov fork [MicroPythona](https://micropython.org/)) za koji su njihovi proizvodi često unaprijed pripremljeni.

{% capture fig_img %}
![arduino logo]({{ '/assets/img/posts/arduino_logo.png' | absolute_url }})
{% endcapture %}
<figure class="align-right" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
</figure>

Naravno, kad se radi o Arduino platformi, neizbježno je spomenuti i njihove [stranice s dokumentacijom](https://docs.arduino.cc/). One uključuju i odličnu [tražilicu biblioteka](https://docs.arduino.cc/libraries/), kao i [priručnik](https://docs.arduino.cc/language-reference/) s popisom funkcija i varijabli koje se koriste kod programiranja Arduino hardvera, što će naročito dobro doći početnicima. Jednako dobar, ako ne i bolji izvor znanja po pitanju Arduina je i [njihov forum](https://forum.arduino.cc/), a tu su i [Arduino Stack Exchange](https://arduino.stackexchange.com/) stranice. 

{% capture fig_img %}
![esp32 logo]({{ '/assets/img/posts/esp32_logo.png' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
</figure>

Veliki broj _embedded_ i _IoT_ projekata danas je baziran na nekoj od varijanti **ESP32** mikrokontrolera, pa je svakako dobro imati pri ruci neke pouzdane izvore vezane za njega. Prvi je ponovno službeni [ESP32 forum](https://www.esp32.com/index.php), kao i [stranica tehničke dokumentacije](https://www.espressif.com/en/support/documents/technical-documents) _Espressifa_, proizvođača ovog mikrokontrolera. Nažalost, niti jedna od ovih stranica nije naročito _user friendly_, naročito za početnike, pa je puno bolje krenuti od [Random Nerd Tutorials](https://randomnerdtutorials.com/) koja pokriva jako puno mogućnosti _ESP32_ mikrokontrolera, a kao bonus ima tutorijale i za _ESP8266_, _Arduino_, _Raspberry Pi_ i _RPi Pico_. Detaljno je objašnjena kako hardverska, tako i softverska strana u svakom primjeru, pa ovo može poslužiti kao odlična osnova za nadogradnju do funkcionalnosti koju želite postići.

Kad smo već kod tutorijala i primjera, evo nekoliko dobrih linkova:
* [instructables.com](https://www.instructables.com/)
* [hackaday.io](https://hackaday.io/projects) (ima tamo i [nas](https://hackaday.io/DIYkits.eu))
* [hackster.io](https://www.hackster.io/)
  
Uzmite u obzir da su neki od članaka na ovim linkovima dosta stari pa budite oprezni jer hardver ili softver na koji se referiraju više ne postoji ili su doživjeli značajne promjene pa upute više nisu aktualne.

{% capture fig_img %}
![raspberry pi logo]({{ '/assets/img/posts/raspberrypi_logo.png' | absolute_url }})
{% endcapture %}
<figure class="align-right" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
</figure>

**Raspberry Pi** je kategorija za sebe, u svakom slučaju treba početi od dokumentacije s [njihovih službenih stranica](https://www.raspberrypi.com/documentation/), a nije loše niti baciti pogled na [Raspberry Pi magazin](https://magazine.raspberrypi.com/). Tu je i [Raspberry Pi Stack Exchange](https://raspberrypi.stackexchange.com/) stranica, kao i [njihov službeni forum](https://forums.raspberrypi.com/), a dobro može doći i [subreddit posvećen RPi platformi](https://www.reddit.com/r/raspberry_pi/). Uz to, [tom's hardware](https://www.tomshardware.com/raspberry-pi/raspberry-pi-projects) prilično redovito donosi članke o raznim Raspberry Pi projektima - nove ideje su uvijek dobrodošle.

{% capture fig_img %}
![youtube logo]({{ '/assets/img/posts/youtube_logo.png' | absolute_url }})
{% endcapture %}
<figure class="align-left" style="margin-top: 0.4em; margin-bottom: 0;width: 300px;">
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
</figure>

Naravno, **YouTube** je neizbježan u ovom popisu, naročito za one koji vše vole vizualnu prezentaciju. Ovdje treba naglasiti da dobar dio kanala nudi linkove na pisanu dokumentaciju i izvorni kod koji se koristi u videu, pa imaju dodatnu vrijednost po tom pitanju. Neki su više okrenuti edukativnoj komponenti i pružaju uvid u širu sliku, a drugi su više specijalizirani, ali svi su izuzetno zanimljivi. Pa, krenimo redom:
* [Andreas Spiess](https://www.youtube.com/@AndreasSpiess) orijentiran je na Arduino/Raspberry Pi/ESP32 komponente, s naročitim naglaskom na komunikaciju (npr. LoRa mrežu)
* [Jeff Geerling](https://www.youtube.com/@JeffGeerling) bavi se najviše Raspberry Pi-em, naročito u kontekstu IT/serverske primjene, ali ne boji se pozabaviti i drugim temama
* [GreatScott!](https://www.youtube.com/@greatscottlab) opisuje razne DIY projekte, više ili manje povezane s Arduino svijetom
* [ElectroBOOM](https://www.youtube.com/@ElectroBOOM) je totalno drugačiji od drugih, ali ne brinite, bez obzira na to što djeluje krajnje neozbiljno, to je samo način na koji dijeli svoje (očito veliko) znanje elektrotehnike
* [ExplainingComputers](https://www.youtube.com/@ExplainingComputers) zahvaća poprilično široko IT područje, ali često se bavi **SBC** (Single Board Computer) platformama, pa je u tom smislu zanimljiv i nama

Na kraju, treba spomenuti i da [Soldered (ex e-radionica)](https://soldered.com/hr/blog/) ima cijeli niz članaka u seriji **KKM (Kako Koristiti Module)** na hrvatskom, što je prava rijetkost. S obzirom na to da su mijenjali platformu koja im je činila osnovu (**Croduino** je postao **Dasduino**), neki članci su možda malo _out-of-date_, ali osnove koje su u njima objašnjene i dalje vrijede, što nikako ne treba zanemariti. One kojima je draže _offline_ iskustvo možemo uputiti na [udrugu Radiona](https://radiona.org/) koja redovito organizira razne radionice, repair shopove i predavanja, često i od strane inozemnih suradnika, pa je to jako dobro mjesto za širenje vlastitih horizonta, čak i ako vam elektronika nije primarni interes.