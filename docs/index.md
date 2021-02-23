---
layout: default
#title: MET Norway Weather API documentation
date: 2020-04-27
author: Geir Aalberg
---

# Index

Dette er en oversikt over ressurser som studentene kan bruke på de forskjellige casene i kurset.

## Generelt

- [Betingelser for bruk av APIet](https://docs.api.met.no/doc/TermsOfService).
  Bruk IFI-proxy mot APIet så slipper dere å tenke på autentisering og unngår
  throttling, og vi kan spore trafikken lettere.
- [Start her](https://docs.api.met.no/doc/GettingStarted): Test ut APIet fra kommandolinjen
- [Generell bruk av APIet](https://docs.api.met.no/doc/usage): Hvordan APIet fungerer, statuskoder o.l.
- [FAQ](https://docs.api.met.no/doc/FAQ): Ofte stilte spørsmål ("hvorfor fungerer ikke...")
- [Yr Utviklerportal](https://developer.yr.no/) inneholder også mye nyttig informasjon

## API-ressurser

- [Generelle ressurser](./0-general)
- [Case 1. Badetemperaturer](./1-badetemp)
- [Case 2. Farevarsler](./2-farevarsel)
- [Case 3. Søk til Havs](./3-drivbane)
- [Case 4. Vektorkart](./4-vektorkart)
- [Case 5. Flynerd-appen](./5-flynerd)
- [Case 6. Åpent case](./6-opencase)

- [Notater fra 2020](./2020)

{% comment %}

## Nyheter

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a><br/>
      <span class="post-meta">{{ post.date | date: "%-d %b %Y" }}</span>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

{% endcomment %}