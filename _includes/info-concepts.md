# {{ include.item.name }}
{:.no_toc}

> {{ include.item.quote }}

{{ include.item.summary }}

{% include toc.html %}

# Appears In
{% for appearance in include.item.appears-in %}
  * {{ appearance }}
{% endfor %}

# Trivia
{% for trivia in include.item.trivia %}
  * {{ trivia }}
{% endfor %}

# Gallery
{% for image in include.item.gallery %}
  ![]({{ image.image-url }})

  {{ image.description }}
{% endfor %}

# References
{% for reference in include.item.references %}
  * {{ reference }}
{% endfor %}
