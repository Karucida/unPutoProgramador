---
layout: post
title:  "Instalar Jekyll"
date: 2019-03-27 21:30
categories: [Jekyll, Blog]
tags: [Jekyll, Blog, Montar, Github, Español]
---

# Jekyll es...
> Jekyll es un generador simple para sitios web estáticos con capacidades de blog; adecuado para sitios web personales, de proyecto o de organizaciones. Fue escrito en lenguaje de programación Ruby por Tom Preston-Werner, el cofundador de GitHub, y se distribuye bajo la licencia de Código abierto MIT. - [Wikipedia](https://es.wikipedia.org/wiki/Jekyll_(computaci%C3%B3n))

Bueno si no os ha quedado claro os miraís la web de [Jekyll](https://jekyllrb.com/)
## ¿Por qué?
Llevaba tiempo con la idea de montar un blog para las 4 tonterías que voy aprendiendo y las 3 que he sé así que se me ocurrio montarlo en [github](https://github.com) con la opción que tienen para tener [páginas estáticas](https://pages.github.com/), iba a ser muy cutre... pero mucho a lo que pense: _A ver Karu, tu eres tonto pero alguien habrá tenido esa idea y se lo habrá currado_ [no busqué mucho](https://lmddgtfy.net/?q=create%20github%20blog) la verdad y me puse a instalarlo ya que me llamava la sencilled para montarlo, que use markdown.

## Instalación
Yo me lo he instalado en ~~ubuntu~~ linux mint
```shell
sudo apt-get install ruby-full build-essential zlib1g-dev


echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

gem install jekyll bundler
```
> Carlos, olé ahí [te has currado](https://jekyllrb.com/docs/installation/ubuntu/) el tutorial de instalación. -Haterino

Lo sé, la verdad no es que me lo haya currado mucho pero nada más llegar a la página de [Jekyll](https://jekyllrb.com/) aparecen estas instrucciones que  **NO**  hay que seguir


**NO HACER CASO**

***
***
###### de verdad no seais tontos y no hagaís caso hasta que os lo diga más abajo

```shell
gem install bundler jekyll
jekyll new my-awesome-site
cd my-awesome-site
```

Y viendo las 4 cosas y pensando que a ser algo más fácil este es mi `history` de comandos:

```
   49  ruby -v
   50  sudo apt-get intall ruby
   51  sudo apt intall ruby
   52  sudo apt install ruby
   53  gem -v
   54  gcc -v
   55  gem install jekyll bundler
   56  sudo gem install jekyll bundler
   57  jekyll new unputoprogramador
   58  sudo apt install jekyll
   59  jekyll new unputoprogramador
   60  cd unputoprogramador/
   61  bundle exec jekyll serve
   62  gem install jekyll bundler
   63  sudo gem install jekyll bundler
   64  bundle exec jekyll serve
   65  ll
   66  cd ..
   67  rm -r unputoprogramador/
   68  ll

```

***
***
**YA PODEÍS HACERME CASO**

Una vez instalado ya se puede crear el proyecto:
```
jekyll new <nombreDelProyecto>
cd <nombreDelProyecto>
bundle exec jekyll serve
```
En mi caso `<nombreDelProyecto>` = `unPutoProgramador` 

_la primera u es en minuscula porque no tengo clase._ 

###### badum tss...


Ahora podremos acceder a nuestro entorno que esta en:
- [http://localhost:4000](http://localhost:4000)

Si no revisad lo que pone tras iniciar el servidor y fijaros en `server address:` :
```shell
Configuration file: /home/karu/<nombreDelProyecto>/_config.yml
            Source: /home/karu/<nombreDelProyecto>
       Destination: /home/karu/<nombreDelProyecto>/_site
 Incremental build: disabled. Enable with --incremental
      Generating... 
       Jekyll Feed: Generating feed for posts
                    done in 0.386 seconds.
 Auto-regeneration: enabled for '/home/karu/<nombreDelProyecto>'
    Server address: http://127.0.0.1:4000/

```

Cada vez que pongais por terminal y en la ruta, se regenerá el proyecto
```shell
Jekyll build
```

Y hasta aquí el primero de los posts sobre [Jekyll](https://jekyllrb.com/).

El siguiente post será de cómo subirlo a github :D


### Chuletas que molan
- [Chuleta de Jekyll](https://devhints.io/jekyll)
- [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

PD: os quiero
