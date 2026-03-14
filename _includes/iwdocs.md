---
layout: default
title: Gallery
---
{%- assign iwdocs = site.data.iwdocs -%}
<div class="iwdocs">
  {% for item in site.data.iwdocs %}
    {% include iwdocs-item.html
      image=item.image
      title=item.title
      description=item.description
    %}
  {% endfor %}
</div>

---
