---
layout: default
#title: IN2000: Case 2. Farevarsler
date: 2021-02-19
author: Geir Aalberg
---

# Case 3. Søk til Havs

Bruk av drivbanesimuleringer for ting i havet

* Kontakt: Vegard Bønes
* Primære datakilder: Drifty
* Sekundære datakilder: Oceanforecast

Drifty ble bl.a. brukt hefting under Helge Ingstad-forliset. Kan brukers til å lokalisere
folk i sjøen ved redningsulykker, eller å simulere drivbaner til oljeutslipp eller store skip i havsnød.

Ideer:

- mann som faller ut fra oljeplattform, må hentes opp med helikopter som må flys fra land
- sende ut skip for å begrense oljeutslipp


Outputformat er enten bilder eller NetCDF-filer. For sistnevnte må man i Kotlin bruke
et [Java-bibliotek](https://www.unidata.ucar.edu/software/netcdf-java/) fra Unidata.
Det må testes av IFI at funker under Kotlin.
Mulig vi kan få til GeoJSON (har dog ikke spesielt god støtte for tid).

Kilder:

- <https://in2000.drifty.met.no/> Basic Auth
- <https://opendrift.github.io/>
- Locationforecast, Nowcast, Oceanforecast, MetAlerts, Routeforecast

Eksempel:

- <https://rest.drifty.met.no/api/simulation/3a33c845-ad4d-4fef-9097-058dc941ddcb/result>

Programvare:

- ncdump
- fimex
