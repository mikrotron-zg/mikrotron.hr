# mikrotron.hr web

Statične web stranice generirane pomoću [Jekylla](https://jekyllrb.com/) i teme [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes).

## Jekyll upute

### Instalacija

Upute za Ubuntu:

```shell
sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

i na kraju:

```shell
gem install jekyll bundler
```

### Inicijalizacija

Skinuti temu koja će se koristiti, prebaciti se u glavni direktorij i pokrenuti

```shell
bundle update
```

pa će se skinuti i instalirati sve potrebno za dotični projekt.

### Lokalni server

Dovoljno je u glavnom direktoriju projekta pokrenuti Jekyll web server:

```shell
jekyll serve
```

### Deployment

Prvo lokalno pokrenuti 

```shell
jekyll build
```

pa onda iskopirati kompletni sadržaj direktorija *_site* na web server u glavni direktorij weba (*www*, *public_html* ili kako se već zove), i to je to.