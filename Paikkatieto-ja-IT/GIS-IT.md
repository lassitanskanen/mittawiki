---
title: GIS-IT
description: Paikkatiedon IT
published: true
date: 2021-11-02T20:25:44.750Z
tags: 
editor: markdown
dateCreated: 2021-11-02T20:09:15.610Z
---

# GIS IT
Asia, jota on hankala nimetä yksiselitteisesti. Tarkemmin selitettynä kyseessä on tietotekniikka geoinformatiikan tieteenalasta, mutta höystettynä maantieteellä ja mittaustekniikalla.

Yksinkertaistettuna GIS IT voisi tarkoittaa selaimessa toimivaa karttapalvelua, joita monella kunnalla nykyään on. Toisaalta taustalla on paljon sellaista logiikkaa, joka ei karttapalvelun käyttäjälle näy, jolloin kattavammin sanottuna puhutaan laajasta IT-kokonaisuudesta.

### Mitä karttapalvelun taustalla sitten on?
Ensimmäisen huulille nousee todennäköisesti [Geoserver](http://geoserver.org/), joka pyörii ehkä useimmassa GIS käyttöön tarkoitetussa palvelimessa. Toisena voisi olla [PostGIS](https://postgis.net/), joka pyörii ehkä eniten GIS käyttöön suunnatuissa tietokannoissa. Käytännössä PostGIS on lisäosa [PostgreSQL](https://www.postgresql.org/) tietokannan päällä. Näiden kahden avulla saa rakennettua kattavan (robustin) taustan mille tahansa GIS-palvelulle.