---
layout: default
title: 'Class Directory'
description: 'CSHL Advanced Sequencing Technologies Course, 2017'
---
## Instructors
{% assign instructors = site.participants | where: 'role', 'Instructor' %}
{% for instructor in instructors %}
  {% include team_member participant=instructor %}
{% endfor %}

* * *

## Teaching Assistants
{% assign tas = site.participants | where: 'role', 'TA' %}
{% for ta in tas %}
  {% include team_member participant=ta %}
{% endfor %}

* * *

## Students
{% assign students = site.participants | where: 'role', 'Student' | where_exp: 'p', 'p.name != "John Q. Student"' %}
{% for student in students %}
  {% include team_member participant=student %}
{% endfor %}
