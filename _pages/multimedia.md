---
title: "WANG-AXIS Lab - Multimedia"
layout: piclay
excerpt: "WANG-AXIS Lab -- Multimedia"
permalink: /multimedia/
---

# Pictures



## Presentations

#### How X-rays see through your skin -- Ge Wang:
<iframe width="640" height="360" src="https://www.youtube.com/embed/gsV7SJDDCY4" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Machine Learning for Tomographic Imaging presented at University of Minnesota
<iframe width="640" height="360" src="https://reel.ima.umn.edu/videos/2019/SW10.14-18.19/Wang-10-16-19.mp4" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Looking Forward as RPI Leads Innovative Cancer Research, Spectrum News
<iframe width="640" height="360" src="https://ns8-ns-twc-com.akamaized.net/news/mpx/133/247/40825778_AL%20Cancer%20Imaging%20Business%20Beat%20PKG.mp4" frameborder="0" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Wang %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
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
