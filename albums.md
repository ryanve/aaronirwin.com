---
title: Albums
permalink: /albums/index.html
---

# Albums

**Stream on [Spotify](https://open.spotify.com/search/albums/%22aaron%20irwin%22), [Bandcamp](https://aaronirwin.bandcamp.com)**

<ol class="pad-0 grid-2">
{% assign albums = (site.albums | sort: "chronology") | reverse %}
{% for item in albums %}
  <li class="block-flow">
    <a class="block-flex flex-column" href="{{ item.url | relative_url }}">
      <img
        alt="{{ item.title }}"
        width="480"
        height="480"
        src="{{ item.cover.min }}" />
    </a>
  </li>
{% endfor %}
</ol>
