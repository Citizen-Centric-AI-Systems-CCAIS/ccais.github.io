---
title: "News | Citizen-Centric AI Systems | University of Southampton"
layout: textlay
excerpt: "News | Citizen-Centric AI Systems | University of Southampton"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}

<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
