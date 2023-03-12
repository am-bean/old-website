---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
---

## News

<div class="jumbotron">
{% for article in site.data.news %}
<b>{{ article.date }}</b>

<h5>{{ article.headline }}<h5>
{% if article.body %} {{article.body}} {% endif %}
{% if article.url %} <a href= {{article.url}} >Link</a> {% endif %}
{% endfor %}
</div>
