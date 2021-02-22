---
layout: default
#title: IN2000: Case 1. Badetemperatur
date: 2021-02-19
author: Geir Aalberg
---

# Case 1. Badetemperatur


* Kontakt: Havvarselprosjektet v/ Martin Lilleeng Sætra
* Primære datakilder: http://havvarsel-frost.met.no (under oppsetting), https://api.met.no (Oceanforecast)
* Sekundære datakilder: https://api.met.no (Locationforecast og Nowcast)

Til våren vil det bli samlet inn "live" observasjoner fra bøyer plassert ved populære
badesteder i Oslo og omegn, og i Bergen. Observasjonene kan så hentes
fra en egen Frost-server hos Meteorologisk institutt.

Inntil bøyene legges ut så kan det gjøres testing med historiske observasjone,
for eksempel fra i fjor sommer. Ved å kombinere observasjoner med
varsler/prognoser fra api.met.no så kan det lages en rekke forskjellige
funksjonalitet rundt temaet badetemperaturer. Noen ideer til inspirasjon:

 - Kart med "live" badetemperaturer plottet inn på kjente badesteder.
 - Rangering av strender etter vanntemperatur, lufttemperatur, minste forskjell i vanntemperatur og lufttemperatur osv.
 - Hvilken tid på døgnet er det mest behagelig å bade?
 - "Push notification" (eller lignende) hvis det måles temperaturer over en viss grense.
 - Hvor gode er varslene/prognosene fra api.met.no til å predikere badetemperaturer? Sammenligning av varsler og observasjoner. (Det nærmeste punktet som det gis varsel for ligger ofte et godt stykke ut i fjorden/havet.)

Vi ønsker også å tilgjengeliggjøre observasjoner som publikum sender
inn til yr.no i samarbeid med
[Reiseradioen](https://www.yr.no/nb/badetemperaturer​). Dette er noe som kanskje
blir lagt til som en ekstra datakilde på havvarsel-frost.met.no i løpet av
våren, i tillegg til flere bøyer.

