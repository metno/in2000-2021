---
layout: default
#title: MET Norway Weather API documentation
#date: 2020-04-27
#author: Geir Aalberg
---

# Ressurser relevante for IN2000 våren 2021

## Generelt

- [Emneside](https://www.uio.no/studier/emner/matnat/ifi/IN2000/v21/)


## Ressurser fordelt på case

- [Case 1. Badetemperaturer](./1-badetemp)
- [Case 2. Farevarsler](./2-farevarsel)
- [Case 3. Søk til Havs](./3-drivbane)
- [Case 4. Vektorkart](./4-vektorkart)
- [Case 5. Flynerd-appen](./5-flynerd)
- [Case 6. Åpent case](./6-opencase)

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
