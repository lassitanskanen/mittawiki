---
title: Handbookit
description: Käytännön mittauksessa on nopeita tilanteita, joissa tarvitaan nopeaa tiedonhakua. Handbookit ovat kategorisoitu kohteen mukaan. Lue online tai tulosta mukaan maastoon!
published: true
date: 2021-05-30T19:08:17.744Z
tags: 
editor: markdown
dateCreated: 2020-07-21T17:53:17.911Z
---

# Handbookit

Kootusti nopeaa tietoa.

# Handbook 1: Koordinaattijärjestelmät Suomessa

Sääntö 1: Älä arvaa koordinaattijärjestelmää.

Suomessa on useita koordinaattijärjestelmiä, joista uusimmat ja modernimmat ovat seuraavat:

- ETRS-TM35FIN (epsg:3067)
	- Koordinaattiesimerkki: 6823365, 326711
	- Esimerkiksi Maanmittauslaitoksen peruskartta.
- ETRS-GKn =
	- Koordinaattiesimerkki: GK24 6821790.6056, 24486330.0922
  - Esimerkiksi kaupunkien omat kartat yms. sijaintipalvelut. Tampereella
	- GK-kaistoja käytetään lähes aina kaikissa rakennusmittauksissa, koska ne ovat tarkempia 
	kuin esimerkiksi ETRS-TM35FIN.
- KKJ (Kartastokoordinaattijärjestelmä)
	- Koordinaattiesimerkki: 
  - Esimerkiksi vanhemmat suunnitelmat
- WGS84 (epsg:4326) = 
	- Koordinaattiesimerkki: 61° 30' 17,883" (lat) 23° 44' 35,841" (lon)
  - Esimerkin muoto on aste, minuutti ja sekunti. Voidaan ilmoittaa myös aste ja minuutti (61° 30,29805' ja 23° 44,59735') tai aste (61,504967488° ja 23,743289185°)
	- GPS mittaa näitä koordinaatteja.

**Termit hukassa?**
- Latitudi (lat) = leveyspiiri
- Longitudi (lon) = pituuspiiri
- Geoidi = merenpinnan "jatke" mantereella. Kuvaa nolla korkoa, koska merenpinta on yleisesti nolla korkeus.

**Muunnospalveluita**
https://kartta.paikkatietoikkuna.fi/?lang=fi
WGS84 muunnospalvelu

# Handbook 2: Korkeusjärjestelmät Suomessa = korkeus geoidimallista.

Sääntö 1: Älä **ikinä** arvaa **korkeus**järjestelmää.

N2000 = nykyinen korkeusjärjestelmä (Geoidimallin nimi on FIN2005)
N60 = vanhempi 1960-luvun korkeusjärjestelmä (Geoidimallin nimi on FIN2000)

HUOM! Ero N2000 ja N60 lukemien välillä on **14-43cm** riippuen sijainnista.

Vanhemmat korkeusjärjestelmät:
N43 = 2. tarkkavaaitus 1935–1975. Tilapäinen korkeusjärjestelmä, johon saattaa vielä joskus
törmätä eri kunnissa.

NN = 1. tarkkavaaitus 1892–1910. Ensimmäinen valtakunnallinen korkeusjärjestelmä. Esiintyy vielä muun muassa vesistöjen säännöstelypäätöksissä ja sisävesien syvyystiedoissa.

# Handbook 3: Ohjelmat

- 3D-WIN (3d-system.fi)
- QGIS (qgis.org)
- Notepad++ (notepad-plus-plus.org)
- Trimble Business Center

# Handbook 4: Tiedostoformaatit ja niiden avaus

- DXF
	- Millä saan auki? 3D-WIN, Trimble Business Center, AutoCAD 3D
  - Vain "tyhmiä" pisteitä ja viivoja eri layereilla. Siivoa ja yksinkertaista ennen mittausta.
- DWG
  - Millä saan auki? 3D-WIN, Trimble Business Center, AutoCAD 3D
  - Vain "tyhmiä" pisteitä ja viivoja eri layereilla. Siivoa ja yksinkertaista ennen mittausta.
- .shp (shapefile)
  - Millä saan auki? 3D-WIN, Trimble Business Center tai QGIS
- .gt (vanha tielaitoksen formaatti)
  - Millä saan auki? 3D-WIN, Trimble Business Center tai Notepad++
- LandXML
	- Millä saan auki? Trimble Business Center ja 3D-WIN: Avaa LandXML
  - http://www.3d-system.net/wiki/index.php/tiedosto/formaatit/20-landxml-tiedostojen-luku


# Handbook 5: Maastomerkintä, merkit rakentajille

Kova pinta
- asfalttinaula
	- käyttö: vasaralla haluttuun kohtaan kuten puunaulatkin
- merkintäsprayt (kaupassa esim. Mercalin RS-merkintämaali)
	- käyttö: suihke tulee pullon päältä
- betoninaula (pöllönsilmä, kaupassa lyöntiniitti)
	- käyttö: porataan ensin reikä kiviporalla, asetetaan betoninaula     		reikään ja vasaroidaan laajentaja sisään.
- liitu, tussi, kynä

Pehmeä pinta
- korkotikku puurimasta (kova maa / sora)
- merkintäsprayt

Korkotikku + korkolappu ilmaisee konekuskille mille korolle maanpinta tulee. Tavallisesti korkolappu laitetaan esim. +0.5m, jolloin konekuski käy mittanauhalla tarkistamassa tilanteen. Hän voi tuoda myös tasolaserin ja asemoi sen vastaamaan mittaamaasi lappua. Sinulla tulee olla autossa aina mukana 
- valmiiksi sahattuja ja teroitettuja puutikkuja (esim. 10kpl 1.5m ja 5kpl 2m)
- korkolappuja (sihtilappu)
- nitoja + niittejä
- kirves
- puusaha
- käsimittanauha
- tusseja sihtilappuun merkkausta varten

*Kuva korkolapusta oikeinpäin*
*Kuva valmiista mittatikusta*

#### Luiskakeppi
Luiskakeppi ilmaisee konekuskille mikä luiskan (piennar, rinne) kaltevuus on.

*Kuva valmiista luiskakepistä*









#### Lähteet:
- Maanmittauslaitos. 20200806 klo. 22:31. https://www.maanmittauslaitos.fi/sites/maanmittauslaitos.fi/files/old/N2000_Valtakunnallinen_korkeusjarjestelma.pdf