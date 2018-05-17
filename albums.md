---
title: Albums
permalink: /albums/index.html
---

# Albums

{% assign albums = (site.albums | sort: "chronology") | reverse %}
{% for item in albums %}
  - [![{{ item.title }}]({{ item.cover.min }})]({{ item.url | relative_url }})
{% endfor %}
