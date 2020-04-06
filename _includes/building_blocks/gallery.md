{% if include.item.gallery %}
# Gallery
{% for image in include.item.gallery %}
  {% include figure.html url=image.image-url text=image.description %}
{% endfor %}
{% endif %}