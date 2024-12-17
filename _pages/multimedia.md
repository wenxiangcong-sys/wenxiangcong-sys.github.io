---
title: "Intellimaging Tech - Multimedia"
layout: piclay
excerpt: "Intellimaging -- Multimedia"
permalink: /multimedia/
---


<br/>
<br/>
<br/>

<!--# Pictures-->



## Presentations

#### AI for Medical Imaging (11/08/2023)
<iframe width="640" height="360" src="https://www.tube.com/embed/iaP5uIBYmGE?si=8EGqudj9qd_orU9v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### Future of Medical Imaging (11/01/2022)
<iframe width="640" height="360" src="https://www.tube.com/embed/qgSVcsaJqKk?si=pQ9f_6ADemTqi-6H" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Gallery
(Click on an Image for Zooming)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Wang %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
  <p>{{ pic.title }}</p>
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" data-lightbox="gallery">
    <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </a>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
