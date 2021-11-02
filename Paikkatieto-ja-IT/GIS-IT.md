---
title: GIS-IT
description: Paikkatiedon IT
published: true
date: 2021-11-02T20:42:14.050Z
tags: 
editor: markdown
dateCreated: 2021-11-02T20:09:15.610Z
---

# GIS IT
Asia, jota on hankala nimetä yksiselitteisesti. Tarkemmin selitettynä kyseessä on tietotekniikka geoinformatiikan tieteenalasta, mutta höystettynä maantieteellä ja mittaustekniikalla.

Yksinkertaistettuna GIS IT voisi tarkoittaa selaimessa toimivaa karttapalvelua, joita monella kunnalla nykyään on. Toisaalta taustalla on paljon sellaista logiikkaa, joka ei karttapalvelun käyttäjälle näy, jolloin kattavammin sanottuna puhutaan laajasta IT-kokonaisuudesta.

### Mitä karttapalvelun taustalla sitten on?
Ensimmäisen huulille nousee todennäköisesti [Geoserver](http://geoserver.org/), joka pyörii ehkä useimmassa GIS käyttöön tarkoitetussa palvelimessa. Toisena voisi olla [PostGIS](https://postgis.net/), joka pyörii ehkä eniten GIS käyttöön suunnatuissa tietokannoissa. Käytännössä PostGIS on lisäosa [PostgreSQL](https://www.postgresql.org/) tietokannan päällä. Näiden kahden avulla saa rakennettua kattavan (robustin) taustan mille tahansa GIS-palvelulle.

### Suomi GIS IT asiaa
Ehkä eniten harmaita hiuksia puhtaalta pöydältä aloittaessa tulee koordinaattijärjestelmistä. Nimittäin joku on päättänyt, että WGS84 (EPSG:4326) on peruskoordinaatisto, kun puhutaan GIS IT asioista. Erityisesti Geoserver on toteutettu niin, että koordinaatteja käsitellään palvelinohjelman sisällä aina y/x järjestyksessä. Eli käytännössä WGS84 lat/lon.

Koko Suomen aineistoissa yleisesti käytetty TM35FIN (EPSG:3067) koordinaatisto toimii kivasti, koska järjestys on päätetty fiksusti y/x. GKn kaistat sen sijaan eivät, koska niissä järjestys on geodeettisesti oikein eli x/y.

Yllä selitetyn voi tarkistaa helposti täältä: [epsg.io](https://epsg.io/)

- TM35FIN sekä järjestys on teknisesti oletusarvo eli **enu**
- GKn kaistojen koordinaattijärjestys on **neu**

Tämä kannattaa muistaa erityisesti javascript PROJ-scripteissä. Edes epsg.io ei tarjoa siten oikeaa tietoa. +axis=neu

---

Toinen asia on GKn kaistojen WMTS toimivuus Geoserverillä.

Ohessa on toimivat GWC gridset konfiguraatiot:

+++++





