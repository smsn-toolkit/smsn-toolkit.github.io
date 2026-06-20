---
layout: default
title: Toolkit Hub
permalink: /toolkit-hub/
---

Welcome to the Accessibility Toolkit.

<!-- **Edit `_data/toolkit.yml` to add, change, or remove an entry on this page**
<!-- NO EDITING OF THIS PAGE IS REQUIRED TO CHANGE ITEMS IN THE LISTS. -->

{% for category in site.data.toolkit %}
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
