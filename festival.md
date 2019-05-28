---
layout: page
title: Festival
permalink: /festival/
---

Yearly festival blah blah blah.

{% for performer in site.performers %}
  {% assign even=forloop.index | modulo: 2 %}
  {% include intro.html performer=performer even=even %}
{% endfor %}