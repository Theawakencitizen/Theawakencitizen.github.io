---
layout: default
---

# Archivos

<ul>
{% for file in site.static_files %}
  {% if file.path contains "/noticias/" %}
    <li><a href="{{ site.baseurl'/noticias/' }}</a></li>
  {% endif %}
{% endfor %}
</ul>
