---
layout: post
title: Coming Soon…
tags: thesystem
---

This will be the home of the public facing part of my memex/zettelkasten

It's being built using jekyll and GitHub pages.

The underlying structure is Living/Earning/Growing.

<span>[
  {% for tag in page.tags %}
    {% capture tag_name %}{{ tag }}{% endcapture %}
    <a href="/tag/{{ tag_name }}"><code class="highligher-rouge"><nobr>{{ tag_name }}</nobr></code>&nbsp;</a>
  {% endfor %}
]</span>

