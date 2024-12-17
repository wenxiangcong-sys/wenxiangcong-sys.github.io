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
        {% if publi.title %}
        <pubtit>{{ publi.title }}</pubtit>
        {% endif %}
        
        {% if publi.image %}
        <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" 
             class="img-responsive" width="33%" style="float: left" />
        {% endif %}
        
        {% if publi.description %}
        <p>{{ publi.description }}</p>
        {% endif %}
        
        {% if publi.authors %}
        <p><em>{{ publi.authors }}</em></p>
        {% endif %}
        
        {% if publi.link.url %}
        <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
        {% endif %}
        
        {% if publi.news1 %}
        <p class="text-danger"><strong>{{ publi.news1 }}</strong></p>
        {% endif %}
        
        {% if publi.news2 %}
        <p>{{ publi.news2 }}</p>
        {% endif %}
      </div>
    </div>

    {% assign number_printed = number_printed | plus: 1 %}
    {% assign even_odd = number_printed | modulo: 2 %}

    {% if even_odd == 0 %}
    </div> <!-- Close row -->
    {% endif %}

  {% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div> <!-- Close last row for odd items -->
{% endif %}

<p>&nbsp;</p>

## Representative Research Articles

<ol>
  {%- for pub in site.data.pub_repres_works -%}
    {% if pub.type == "works" %}
    <li>
      <p>
        {% if pub.title %}
        <b>{{ pub.title | replace: "&#58;", ":" }}</b><br>
        {% endif %}
        
        {% if pub.author %}
        {{ pub.author }}<br>
        {% endif %}
        
        {% if pub.venue %}
        {{ pub.venue | replace: "&#58;", ":" | capitalize }}<br>
        {% endif %}
        
        {% if pub.url %}
        [<a href="{{ pub.url }}">link</a>]
        {% endif %}
      </p>
    </li>
    {% endif %}
  {%- endfor -%}
</ol>

<p>&nbsp;</p>
