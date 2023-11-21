---
title: "Teaching"
layout: gridlay
sitemap: false
permalink: /teaching/
---

## Teaching

{% for course in site.data.courses %}
<div>
<div class="jumbotron">
<h4>{{ course.name }}</h4>
</div>
<p>{{ course.role }} </p>
<p>{{ course.location }}</p>
<p>{{ course.terms }}</p>
{{ course.description }}

<p>{% if course.github %} <a href="{{ course.github }}" target="_blank"><i class="fa fa-github-square fa-3x" style="margin-right:5px"></i></a>{% endif %}
{% if course.coursepage %} <a href="{{ course.coursepage }}" target="_blank"><i class="fa fa-external-link fa-3x" style="margin-right:5px"></i></a>{% endif %}
</p>
</div>
{% endfor %}



