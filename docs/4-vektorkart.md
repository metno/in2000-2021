---
layout: default
#title: IN2000: Case 2. Farevarsler
date: 2021-02-19
author: Geir Aalberg
---


# 4. Vektorkart

Vær med å teste ny kartløsning for Yr! MET holder på å lage en prototype for vektorkart,
og dere skal lage en klient for denne. Det finnes har mange mulige datakilder, for eksempel:

- temperatur, vind og nedbør i timesoppløsning for Norden
- temperatur, vind og nedbør i 6-timesoppløsning for hele verden
- nedbørsskyer i tilnærmet sanntid (nåvarsel)

Mulige ideer:

- Nedbørskart à la Yr med animerte regnbyger
- Vis temperaturkart for hele verden for å planlegge hvor man bør dra på sommerferie (post-Corona)
- Sykkelkart for Oslo med sykkelstier og fare for regn

Kartserveren leverer vektordata på mapbox format (protobuf) samt JSON metadata.
Klienten kan bruke Javascript eller native Android Mapbox-bibliotek (ikke testet under Kotlin).
Teamene kan selv velge bakgrunnskart (vi anbefaler OpenStreetMap) og må rendre
datalagene oppå dette.

Dette kreves at man setter seg litt inn i forskjellige kartprojeksjoner og
forskjellen på inner/outer polygon (hvilken vei de roterer), se dokumentasjon.

## Datakilder

Primær (obligatorisk):

- [Testserver](https://test.openmaps.met.no/in2000/map/services) for IN2000
  - <https://test.openmaps.met.no/in2000/map/> (prototype på webklient)
  - <https://test.openmaps.met.no/in2000/map/services> (API)
  - <https://gitlab.met.no/yr-maps/maps-frontend-2020/> (intern kodebase)

Sekundære (valgfritt):

- Locationforecast
- Nedbørskart
- MetAlerts
- Sykkelstier med koordinater fra Oslo Kommune

## Dokumentasjon

Mapbox protokoll og biblioteker:

 - Vector tile specification: <https://github.com/mapbox/vector-tile-spec/>
 - Native bibliotek for Android og andre OS (iOS/MacOS): <https://github.com/mapbox/mapbox-gl-native>
 - Javascript biblioteker:
   - Mapbox GL <https://github.com/mapbox/mapbox-gl-js>
   - Openlayers <https://openlayers.org/>
   - Leaflet <https://leafletjs.com/>

Kontakt: [Børge Moe](mailto:borgem@met.no)
