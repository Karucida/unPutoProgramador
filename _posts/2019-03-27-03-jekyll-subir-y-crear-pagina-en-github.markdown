---
layout: post
title:  "#03 Jekyll - Subir y crear página en github"
date: 2019-03-27 20:46
categories: [Jekyll, Blog]
tags: [Jekyll, Blog, Montar, Github, Español]
---

# Subir y crear página en Github

### Crear git
Dentro de nuestro git vamos a new
![Crear página en github](/assets/img/03/2019-03-27creargit1.png)
Una vez rellenamos la configuración inicial
![Crear página en github]({{site.baseurl}}/assetsimg/03/2019-03-27creargit2.png)

Nos vamos a nuestra maquina donde tenemos el blog
```
cd <ruta>/<nombreDelProyecto>
```
En mi caso es /home/karu/unPutoProgramador

editamos \_config.yml y en `baseurl` ponemos `<nombreDelProyecto>` en mi caso unPutoProgramdor

Hacemos que el proyecto sea con el control de versiones git:
```shell
git init
```
Ahora vamos a decirle a git dónde esta el repositorio de github que es lo que nos pone nada más crear el proyecto github
```shell
git remote add origin https://github.com/Karucida/unPutoProgramador.git
```
Añadimos todos los ficheros commiteamos (no sé si existe ese palabro) y pusheamos
```shell
git add --all
commit -m "comenzamos blog"
git push origin master
```
Ya lo tenemos subido!!

Ahora vamos a decirle a github que queremos hacer ese repo vamos a `Settings` de repo y bajamos hasta encontrar `GitHub Pages`
![Crear página en github]({{ site.url }}/assets/img/03/2019-03-27crearpagina.png)

Donde pone `Source`>`None` yo voy a seleccionar la rama master `master branch`

Ya tenemos nuestra página subida!!!

[https://karucida.github.io/unPutoProgramador/](https://karucida.github.io/unPutoProgramador/)

PD:os quiero

