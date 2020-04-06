# {{ include.item.name }}
{:.no_toc}

> {{ include.item.quote }}

{% include toc.html %}

{{ include.item.summary }}

# Biology
{{ include.item.biology }}

# Background
{{ include.item.background }}

# Notable Individuals
{% for individual in include.item.notable-individuals %}
  * {{ individual }}
{% endfor %}

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
  {% include figure.html url=image.image-url text=image.description %}
{% endfor %}

# References
{% for reference in include.item.references %}
  * {{ reference }}
{% endfor %}
