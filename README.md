# Participants

## Instructors
{% assign instructors = site.participants | where: 'role', 'instructor' %}
{% for instructor in instructors %}
  {% include team_member participant=instructor %}
{% endfor %}

## Teaching Assistants
{% assign tas = site.participants | where: 'role', 'ta' %}
{% for ta in tas %}
  {% include team_member participant=ta %}
{% endfor %}

## Students
{% assign students = site.participants | where: 'role', 'student' %}
{% for student in students %}
  {% include team_member participant=student %}
{% endfor %}