---
layout: page
title: VEM MONSTRO
permalink: /etapas/
order: 1
---

<h2>Etapas do Projeto:</h2>


{% for gallery in site.galleries %}
- [{{ gallery.description }}]({{ gallery.id }})
{% endfor %}

