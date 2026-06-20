---
layout: default
title: External Links
permalink: /external-links/
---

These additional links may also be useful.

<!-- 
To add, edit, or remove a link, you only need to 
edit `_data/links.yml` — this page builds itself
from that file automatically.
-->

{% for category in site.data.links %}
### {{ category.category }}

<div class="columns is-multiline">
{% for item in category.items %}
  <div class="column is-half">
    <a class="box link-card" href="{{ item.url }}" target="_blank" rel="noopener">
      <p class="title is-5">{{ item.title }}</p>
      <p class="subtitle is-6 mb-0">{{ item.description }}</p>
    </a>
  </div>
{% endfor %}
</div>
{% endfor %}
