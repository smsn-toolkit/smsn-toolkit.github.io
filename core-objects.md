---
layout: default
title: Core Objects
permalink: /core-objects/
---

This page is dedicate to core objects like images, diagrams, plots, tables and other artifacts used across all your learning resources.

<!-- 
To add, edit, or remove a link, you only need to 
edit `_data/core-objects.yml` — this page builds itself
from that file automatically.
-->

{% for category in site.data.core %}
## {{ category.category }}
{: .title .is-4}

<div class="columns is-multiline">
{% for item in category.items %}
  <div class="column is-half">
    <a class="box link-card" href="{{ item.url }}">
      <p class="title is-5">{{ item.title }}</p>
      <p class="subtitle is-6 mb-0">{{ item.description }}</p>
    </a>
  </div>
{% endfor %}
</div>
{% endfor %}
