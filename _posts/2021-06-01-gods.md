---
layout: post
title:  "the Gods of Oda"
author: ali-bobby
categories: [ polychrome, indices ]
image: assets/images/gods/tredectheon-splash.png
summary: "the Tredectheon"
---

## the Thirteen Major Gods
<div class='grid-section'>
{% assign sorted_posts = site.posts | sort:'title' %}
{% for post in sorted_posts  %}
{% if post.categories contains "polychrome" and post.categories contains "gods" %}

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
