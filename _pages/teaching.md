---
title: "Teaching"
layout: gridlay
sitemap: false
permalink: /teaching/
---

## Teaching

{% for course in site.data.courses %}
<div class="jumbotron">
<h4>{{ course.name }}</h4>
<p>{{ course.location }} ({{ course.terms }})</p>
{{ course.description }}
<p>{% if course.github %} [View on Github]({{course.github}}){% endif %}</p>
</div>
{% endfor %}



