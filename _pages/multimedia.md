---
title: "WANG-AXIS Lab - Multimedia"
layout: piclay
excerpt: "WANG-AXIS Lab -- Multimedia"
permalink: /multimedia/
---


<br/>
<br/>
<br/>

<!--# Pictures-->



## Presentations

#### Tribute to Prof. Ulrich Bonse (Ge Wang presented on 08/22/2024; avatarized by Mr. Md Zabirul Islam on 08/25/24)
<iframe width="640" height="360" src="https://www.youtube.com/embed/FGTP0W3RTiA?si=VO1rQdq4Y8vMRWR4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### Foundation Models in Medicine (08/19/2024)
<iframe width="640" height="360" src="https://www.youtube.com/embed/Yjfjhvl0ktw?si=hD1cKVFPOVuwSjrb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### AI for Medical Imaging (11/08/2023)
<iframe width="640" height="360" src="https://www.tube.com/embed/iaP5uIBYmGE?si=8EGqudj9qd_orU9v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### First Place of the 2023 AAPM DGM Image Generation Challenge (07/27/2023)
<iframe width="640" height="360" src="https://www.tube.com/embed/_6fCqpj8zjE?si=Nu9QG8MNkNsRf3GY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### Deep Learning with Diffusion and Large Models (05/25/2023)
<iframe width="640" height="360" src="https://www.tube.com/embed/m4DvhHlY0Xg?si=K0uWXEge5EJ4dlk7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

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
