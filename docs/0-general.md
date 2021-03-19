---
layout: default
#title: IN2000: Case 1. Badetemperatur
date: 2021-02-19
author: Geir Aalberg
---

# Generelle ressurser

Disse produktene kan være nyttige for alle caser. Data fra disse utgjør størsteparten av det som vises på Yr.
Med unntak av Frost kan alle nås via in2000-apiproxy; for Frost er det satt opp en egen proxy dersom dere ønsker å bruke denne.
Det er ikke nødvendig å bruke proxy for Havvarsel-Frost (case 1).

**NB: IFI-proxyene håndterer ikke `If-Modified-Since`.** Ignorer alt som står om dette i Terms of Service og HOWTO.

## METs åpne datapolitikk

- <https://www.met.no/frie-meteorologiske-data/frie-meteorologiske-data>

## Locationforecast

Globalt værvarsel i times (Norden neste 60 timer) og 6-timers intervaller.

- [Locationforecast/2.0](https://api.met.no/weatherapi/locationforecast/2.0/documentation). Bruk *complete* eller *compact* variant.
- [JSON dataformat](https://docs.api.met.no/doc/ForecastJSON) med
  [eksempel](https://api.met.no/weatherapi/locationforecast/2.0/complete?lat=60.10&lon=9.58)
- [Datamodell](https://docs.api.met.no/doc/locationforecast/datamodel) med forklaring av variabler
- [Locationforecast FAQ](https://docs.api.met.no/doc/locationforecast/FAQ): Ofte stilte spørsmål

## Nowcast

Værvarsel for Norge neste 15 minutter, basert på nedbørsradar og temperaturkorrigert med NetAtmo. Samme format som Locationforecast.

- [Nowcast/2.0](https://api.met.no/weatherapi/nowcast/2.0/documentation) med
  [eksempel](https://api.met.no/weatherapi/nowcast/2.0/complete?lat=59.9333&lon=10.7166)
- [Datamodell](https://docs.api.met.no/doc/nowcast/datamodel) med forklaring av variabler

## Oceanforecast

Havvarsel for Norskekysten.

- [Oceanforecast/0.9](https://api.met.no/weatherapi/oceanforecast/0.9/documentation): Gammel versjon, fases ut til sommeren
  - [Eksempel](https://api.met.no/weatherapi/oceanforecast/0.9/?lat=60.10&lon=5) (XML)
  - [Ditto som JSON](https://api.met.no/weatherapi/oceanforecast/0.9/.json?lat=60.10&lon=5) (autokonvertert)
- [Oceanforecast/2.0](https://api.met.no/weatherapi/oceanforecast/2.0/documentation): Ny JSON versjon, kommer som beta i mars

## Sunrise

Viser når sol og måne går opp/ned over horisonten. Kan også vise avanserte astronomiske
posisjoner for beregning av horoskop(!). Data leveres som XML eller JSON.

- [Sunrise API](https://api.met.no/weatherapi/sunrise/2.0/documentation)

## Frost

MET API for observasjoner og klimadata.

- [Frost API](https://frost.met.no/) - krever registrering og HTTP Basic Auth

Merk at Frost er under omskriving og vil skifte fra versjon 0 til versjon 1 ca 1. april.
Det jobber med å skrive et kompatibilitetslag for å sørge for at eksisterende spørringer
fortsatt vil virke, men for å unngå å måtte endre appen deres ambefaler vi ikke bruk av
Frost i dette semesteret.

## Farevarsler

Se [case 2](./2-farevarsel) for informasjon.
