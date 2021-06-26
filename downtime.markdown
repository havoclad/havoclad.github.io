---
layout: page
title:  Downtime
permalink: /downtime
---

#### Roll after spending your downtime and picking what lifestyle you are going for


| Activity | Downtime | Cost | Benefit | Description |
| --- | --- | --- | --- | --- |
| Training | 1 | 25gp | Go up a level | Psych: remind me to edit this out after testing |
{% assign activities = site.data.downtime %}
{%- for activity in activities -%}
  | {{activity.name}} | {{activity.downtime}} | {{activity.cost}} | {{activity.benefit}} | {{ activity.description }} |
{% endfor %}

Other stuff and things.
