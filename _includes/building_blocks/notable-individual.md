{% if include.item.notable-individuals %}
# Notable Individuals
{% for individual in include.item.notable-individuals %}
  * {{ individual }}
{% endfor %}
{% endif %}