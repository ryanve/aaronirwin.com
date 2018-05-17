---
title: Albums
permalink: /albums/index.html
---

# Albums

<ol class="pad-0">
{% assign albums = (site.albums | sort: "chronology") | reverse %}
{% for item in albums %}
  <li class="block-flow">
    <a href={{ item.url | relative_url }}>
      <img
        alt="{{ item.title }}"
        width="480"
        height="480"
        src="{{ item.cover.min }}" />
    </a>
  </li>
{% endfor %}
</ol>
