{% if include.item.gallery %}
# Gallery

<ul id="image_gallery">
{% for image in include.item.gallery %}
  <li>
{% include figure.html url=image.image-url text=image.description %}
  </li>
{% endfor %}
</ul>
{% endif %}