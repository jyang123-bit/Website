---
layout: category
title: Projects


---

<div class="projects">
{% for projects in site.data.projects %}
- [{{ projects.title }} by {{ projects.program }}]({{ projects.url }})
{% endfor %}
</div>
