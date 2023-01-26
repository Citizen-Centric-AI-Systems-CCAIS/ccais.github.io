---
title: "Publications | Citizen-Centric AI Systems | University of Southampton"
layout: gridlay
excerpt: "Publications | Citizen-Centric AI Systems | University of Southampton"
sitemap: false
permalink: /publications/
---

# Publications

<!-- ## Highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?user=I8dpTJMAAAAJ&hl=en).

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}

<div class="row">
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

## Full List -->

{% assign pub_year = 0 %}

{% for publi in site.data.publist %}

{% if publi.year != pub_year %}
## {{ publi.year }}
{% assign pub_year = publi.year %}
{% endif %}

{{ publi.harvard }}</div> <!-- everything but close divs is rendered fine -- so not sure why this is necessary -->

<!-- For once we have the new publication format  -->
<!--
<a href="{{ publi.link.url }}">{{ publi.title }}</a><br />
{{ publi.authors }}, ({{ publi.year }}). 
-->
<!-- <em>{{}}</em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a> -->

{% endfor %}
