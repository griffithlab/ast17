# Instructors
{% assign instructors = site.participants | where: 'role', 'Instructor' %}
{% for instructor in instructors %}
  {% include team_member participant=instructor %}
{% endfor %}