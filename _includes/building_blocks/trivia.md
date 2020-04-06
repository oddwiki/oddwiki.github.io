{% if include.item.trivia %}
# Trivia
{% for trivia in include.item.trivia %}
  {{ trivia }}
{% endfor %}
{% endif %}