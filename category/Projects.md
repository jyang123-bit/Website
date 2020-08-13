---
layout: category
title: Projects


---

<div class="booklist">
{% for projects in site.data.projects %}
- [{{ projects.title }} by {{ projects.program }}]({{ projects.url }})
{% endfor %}
</div>
