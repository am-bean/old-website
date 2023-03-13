---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
---

## News


{% for article in site.data.news %}
<div class="jumbotron">
<b>{{ article.date }}</b>

<h5>{{ article.headline }}</h5>
{% if article.body %} {{article.body}} {% endif %}
{% if article.url %} 
[Link]({{article.url}}) 
{% endif %}
</div>
{% endfor %}

