---
layout: page
title: Portfolio
---

<h2>dir1 specific header</h2>
<p>dir1specific content. bla bla bla.</p>
{% for page in site.pages %}
  <h3><a title="{{ page.title }}" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a></h3>
  <p>{{page.excerpt}}</p>
{% endfor %}  