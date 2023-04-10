---
layout: default
---

# Archivos

<ul>
{% for file in site.static_files %}
  {% if file.path contains "https://theawakencitizen.github.io" %}
    <li><a href="{{ site.baseurl }}{{ file.path }}">{{ file.path | replace: 'https://theawakencitizen.github.io', '' }}</a></li>
  {% endif %}
{% endfor %}
</ul>
