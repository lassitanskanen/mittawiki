---
title: Paikkatietoanalyysit
description: Perusteet analyyseistä
published: true
date: 2021-11-02T20:05:22.850Z
tags: 
editor: markdown
dateCreated: 2021-05-04T20:06:01.788Z
---

# Paikkatietoanalyysit
Paikkatietoanalyyseillä tarkoitetaan lähtötietojen jalostamista uudeksi tiedoksi. Esimerkiksi tietyn asuinrakennusten etäisyyden lähimmästä yleisestä tiestä voisi olla yksi paikkatietoanalyysi.

## Yleisimmät käyttökohteet

- Intersect eli leikkaavuus
Tehtävänä on esimerkiksi selvittää montako risteystä on tietyllä matkalla. Lähtötiedoiksi otetaan tieverkko josta otetaan haluttu pätkä tietä. Analyysille syötetään tiepätkä ja loppu tieverkko. Muodostuu esimerkiksi pisteaineisto risteyspisteistä.

- Saavutettavuusanalyysi
Tehtävänä on esimerkiksi selvittää kuinka laajalta alueelta yhdelle metrolaiturille pääsee viidessä minuutissa. Lähtötiedoiksi otetaan katu/tieverkko viivoina ja metrolaituri pisteenä. Analyysi tuottaa segmentit esimerkiksi minuutin välein perustuen tiettyyn kävelyvauhtiin.

- Shortest path finder
Tehtävänä on esimerkiksi selvittää lyhin matka pisteestä A pisteeseen B. Lähtötiedoiksi katu/tieverkko ja alku sekä loppupisteet. Analyysi hakee lyhimmän reitin ja antaa sen pituuden.



## Analyysin apumenetelmiä

- Buffer, puskurivyöhykkeen käyttäminen
Puskurivyöhykettä tarvitaan esimerkiksi silloin, kun tarvitaan hakea viivamaisen geometrian lähellä olevia kohteita. Tällöin viivalle voidaan muodostaa prosessinaikainen puskuri ja ajaa sen jälkeen leikkaavuuskysely käyttäen puskuroitua viivaa ja pisteaineistoa. Hyvin hyödyllinen tapa saada esim. kymmenen metrin päässä radan keskilinjasta olevat kohteet selville.
