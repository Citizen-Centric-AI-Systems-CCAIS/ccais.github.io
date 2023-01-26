---
title: "Partners | Citizen-Centric AI Systems | University of Southampton"
layout: gridlay
excerpt: "Partners | Citizen-Centric AI Systems | University of Southampton"
sitemap: false
permalink: /partners/
---


{% assign number_printed = 0 %}
{% for member in site.data.partners %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/partners/{{ member.photo }}" class="img-responsive" width="50%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.bio }}</i>
  <br>
  <!-- <i>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">


  </ul>
  <br>
  <br>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}

</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}

</div>
{% endif %}
