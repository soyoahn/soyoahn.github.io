<div class="gallery">
  {% for item in site.data.gallery %}
    {% include gallery-item.html
      image=item.image
      title=item.title
      description=item.description
    %}
  {% endfor %}
</div>
