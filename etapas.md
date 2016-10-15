---
title: VEM MONSTRO
permalink: "/etapas/"
layout: page
order: 1
---

<h2>Etapas do Projeto:</h2>


<ol type="I">
<li>Compra dos acess&oacute;rios</li>
<p>Uns mimos para enfeitar o pav&atilde;o.</p>
<li>Compra dos opcionais europeus e norte-americanos</li>
<p>A ideia &eacute; customizar o carro deixando o mais original poss&iacute;vel. Ent&atilde;o, ser&atilde;o utilizados opcionais originais dos VW Golf mk3 vendidos na Europa e nos EUA/M&eacute;xico.</p>
<li>Compra do carro</li>
<p>A parte principal e mais delicada do projeto, escolher um carro bom, bonito e barato. :-P</p>
<li>Instala&ccedil;&atilde;o</li>
<p>A hora da divers&atilde;o, onde filho chora e m&atilde;e n&atilde;o ouve, onde a porrada come e ningu&eacute;m v&ecirc;.</p>
</ol>

<h2>Acess&oacute;rios</h2>

{% include galheader.html %}

<p>default header for all gallery pages</p>

{% for gallery in site.data.galleries %}
  {% if gallery.id == page.galleryid %}
    <h1>{{ gallery.description }}</h1>
    <ol>
    {% for image in gallery.images %}
      <li>
        {{ image.text }}<br>
        <a href="{{ gallery.imagefolder }}/{{ image.name }}" data-lightbox="{{ gallery.id }}" title="{{ image.text }}">
          <img src="{{ gallery.imagefolder }}/{{ image.thumb }}">
        </a>
      </li>
    {% endfor %}
    </ol>
  {% endif %}
{% endfor %}