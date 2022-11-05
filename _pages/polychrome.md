---
title: "Polychrome"
layout: default
permalink: "/polychrome.html"
---
<div class="container" markdown='1'>

<div class='display-1 font-weight-bold'> Polychrome </div><br>

<br>

<div class="row align-items-center bg-light" markdown='1'>
<div class="col-md" markdown='1'>
![](/assets/images/places/oda/oda-splash.png)
</div>
<div class="col-md align-items-center" markdown='1'>

## the Terrible World of Oda
Oda. A world in flux. A world where the past is lost, and the future is uncertain. Immense cities rise from the shores, while the dark forests and jungles of the interior remain unexplored. Behemoth creatures emerge from seas and caves, while ghosts lurk in the shadows collecting secrets.

Oda. A terrible world.

[Read more...](/oda)

</div>
</div>

<br>

## Races
There are many intelligent humanoid species on Oda. Humans are by far the most common, numbering in the many millions. Some species are on the verge of extinction, with just hundreds or even dozens of individuals still living.
<div class='grid-section'>
{% assign sorted_posts = site.posts | sort:'title' %}
{% for post in sorted_posts  %}
{% if post.categories contains "polychrome" and post.categories contains "races" %}

<div class="card" style="">
  <img class="card-img-top" src='{{site.url}}/{{post.image}}' alt="{{post.title}}">
  <div class="card-body">
    <h5 class="card-title">
      {{post.title}}
    </h5>
    <p>{{post.summary}}</p>
    <a href="{{post.url}}">Read more...</a>
  </div>
</div>
{% endif %}
{% endfor %}
</div>


---

<div class="container" markdown='1'>
## Equipment
<div class='row'>
{% for post in site.posts %}
{% if post.categories contains "polychrome" and post.categories contains "equipment" %}

<div class="card" style="width: 18rem; margin: 1rem;">
  <img class="card-img-top" src='{{site.url}}/{{post.image}}' alt="{{post.title}}">
  <div class="card-body">
    <h5 class="card-title">
      {{post.title}}
    </h5>
    <p>{{post.summary}}</p>
    <a href="{{post.url}}">Read more...</a>
  </div>
</div>
{% endif %}
{% endfor %}
</div>
