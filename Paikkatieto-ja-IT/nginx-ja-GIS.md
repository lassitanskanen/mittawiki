---
title: Nginx ja GIS
description: 
published: true
date: 2021-11-02T20:48:53.338Z
tags: 
editor: markdown
dateCreated: 2021-11-02T20:48:53.338Z
---

# Nginx ja GIS
Karttapalvelun selaimelle puskee tavallisesti web server palvelinohjelma. Paras tähän on EngineX (NGINX), joka osaa tehdä monenlaisia asioita.

### QGIS-server ja NGINX reverse proxy
Palvelimella kannattaa käyttää mikroservice teknologiaa, esim Docker, jotta eri palvelinohjelmat ovat helpommin hallittavissa ja ylläpidettävissä. Docker Stack on esimerkiksi helppo orkestrointimenetelmä kevyeen käyttöön.

QGIS-serverin eteen kannattaa asettaa NGINX reverse proxy, joka välittää kyselyt FCGI-protokollalla QGIS-serverille.

