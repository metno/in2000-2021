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

* Kontakt: Børge Moe
* Primære datakilder: <https://test.openmaps.met.no/in2000/map/services>
* Sekundære datakilder: Farevarsler?

Kartserveren leverer vektordata på mapbox format (protobuf) samt json metadata. Klienten kan bruke Javascript eller native Mapbox-bibliotek under Kotlin. Teamene kan selv velge bakgrunnskart (vi anbefaler OpenStreetMap) og må rendre datalagene oppå dette. Dette krever noe kjennskap til forskjellige kartprojeksjoner og forskjell på inner/outer polygon (hvilken vei de roterer), se dokumentasjon.

Kilder:

- <https://test.openmaps.met.no/in2000/map/> (testserver)
- <https://test.openmaps.met.no/in2000/map/services> (testserver)
- <https://gitlab.met.no/yr-maps/maps-frontend-2020/> (intern kodebase)

Mapbox:

 - Vector tile specification: <https://github.com/mapbox/vector-tile-spec/>
 - Native bibliotek for Android og andre OS (iOS/MacOS): <https://github.com/mapbox/mapbox-gl-native>
 - Javascript:
   - Mapbox GL <https://github.com/mapbox/mapbox-gl-js>
   - Openlayers <https://openlayers.org/>
   - Leaflet <https://leafletjs.com/>
