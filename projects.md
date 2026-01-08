---
layout: page
title: Projects
---

{% for project in site.projects %}

## [{{ project.title }}]({{ project.url }})

{{ project.description | markdownify }}

{% if forloop.last == false %}
---
{% endif %}

{% endfor %}
