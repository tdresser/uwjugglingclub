---
layout: page
title: Show
permalink: /
redirect_from:
  - /show
---

Our incredible Gala Show will be at 7:30pm on Saturday night, with doors opening at 7:00.

Tickets will be $15 for adults and $7 for children 12 and under!

Tickets, or a package including a show ticket and a festival shirt, will be available at the festival and the door (as long as shirt supplies last). 

Alternatively, show tickets will be available online closer to the show date.

{% for performer in site.performers %}
  {% assign even=forloop.index | modulo: 2 %}
  {% include intro.html performer=performer even=even %}
{% endfor %}