---
title: "Intellimaging Tech - Publications"
layout: gridlay
excerpt: "Intellimaging Tech -- Publications."
sitemap: false
permalink: /publication/
---
<br/>
<br/>
<br/>


For a full list see [Google Scholar Profile.](https://scholar.google.com/citations?user=MWsIcikAAAAJ&hl=en)
Codes are publicly available at [Intellimaging Github](https://github.com/wenxiangcong-sys)


## Highlights

{% assign number_printed = 0 %}
{% for publi in site.data.highlights %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row row-flex row-flex-wrap">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Representative Research Articles

<!--<ol reversed>-->
<ol>
{%- for pub in site.data.pub_repres_works -%}
{% if pub.type == "works" %}
<li>
<p> <b>{{ pub.title | replace: "&#58", ":" }}</b><br>
  {{ pub.author }}<br>
  {{ pub.venue | replace: "&#58", ":" | capitalize_all }}<br>
  {%- if pub.url -%}
  [<a href="{{ pub.url}}">link</a>]
  {%- endif -%}
</p>
</li>
{% endif %}
{%- endfor -%}

</ol>

<p> &nbsp; </p>
