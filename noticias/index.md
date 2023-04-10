---
layout: default
---

# Archivos

<ul>
{% for file in site.static_files %}
  {% if file.path contains "/carpeta/" %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.path | replace: '/carpeta/', '' }}</a></li>
  {% endif %}
{% endfor %}
</ul>
