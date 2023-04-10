---
layout: default
---

# Archivos

<ul>
{% for file in site.static_files %}
  {% if file.path contains "./" %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.path | replace: './', '' }}</a></li>
  {% endif %}
{% endfor %}
</ul>
