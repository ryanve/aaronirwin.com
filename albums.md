---
title: Albums
permalink: /albums/index.html
---

# Albums

<ol class="pad-0">
{% assign albums = (site.albums | sort: "chronology") | reverse %}
{% for item in albums %}
  <li class="block-flow">[![{{ item.title }}]({{ item.cover.min }})]({{ item.url | relative_url }})
{% endfor %}
</ol>
