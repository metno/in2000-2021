---
layout: default
#title: IN2000: Case 1. Badetemperatur
date: 2021-02-19
author: Geir Aalberg
---

# Case 1. Badetemperatur

Lag en app som viser badetemperaturer på badeplasser langs Norskekysten.

Til våren vil det bli samlet inn "live" observasjoner fra bøyer plassert ved populære
badesteder i Oslo og omegn, og i Bergen. Observasjonene kan så hentes
fra en egen Frost-server hos Meteorologisk institutt.

Inntil bøyene legges ut så kan det gjøres testing med historiske observasjone,
for eksempel fra i fjor sommer. Ved å kombinere observasjoner med
varsler/prognoser fra api.met.no så kan det lages en rekke forskjellige
funksjonalitet rundt temaet badetemperaturer.

Vi ønsker også å tilgjengeliggjøre observasjoner som publikum sender
inn til yr.no i samarbeid med
[Reiseradioen](https://www.yr.no/nb/badetemperaturer​). Dette er noe som kanskje
blir lagt til som en ekstra datakilde på havvarsel-frost.met.no i løpet av
våren, i tillegg til flere bøyer.

## Noen ideer til inspirasjon:

 - Kart med "live" badetemperaturer plottet inn på kjente badesteder.
 - Rangering av strender etter vanntemperatur, lufttemperatur, minste forskjell i vanntemperatur og lufttemperatur osv.
 - Hvilken tid på døgnet er det mest behagelig å bade?
 - Hvor gode er varslene/prognosene fra api.met.no til å predikere
   badetemperaturer? Sammenligning av Oceanforecast-varsler og observasjoner. (Det nærmeste
   punktet som det gis varsel for ligger ofte et godt stykke ut i
   fjorden/havet, så bruk Oceanforecast 2.0 beta som automatisk "snapper" til nærmeste punkt)

## Datakilder

Primære (obligatisk):

- [Havvarsel-Frost](http://havvarsel-frost.met.no) (under oppsetting)
- Oceanforecast (se generelt)

Sekundære (valgfritt):

- Locationforecast
- Nowcast
- [Oslo Kommune](https://www.oslo.kommune.no/natur-kultur-og-fritid/tur-og-friluftsliv/badeplasser-og-temperaturer/)
- [Badevann.no](https://badevann.no/)

## Kontakt

Havvarselprosjektet v/ [Martin Lilleeng Sætra](mailto:martinls@met.no) (for tekniske spørsmål rundt Havvarsel-Frost)

