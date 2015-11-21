---
layout: page
title: Digital Portfolio
---

<p>Aleksandr Beliaev's digital portfolio for Tallinn University HCI Master Programme</p>
{% for page in site.pages %}
  {% if page.sampleno %}
<h3><a title="{{ page.title }}" href="{{ page.url | prepend: site.baseurl }}"><strong>Sample {{ page.sampleno }}.</strong> {{ page.title }}</a></h3>
<p>{{page.excerpt}}</p>
  {% endif %}
{% endfor %}  