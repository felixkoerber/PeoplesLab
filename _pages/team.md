---
title: Team
subtitle: Meet the people in the lab
permalink: /team
layout: page
---

{% assign team_members = site.team | sort: 'name' %}

{% if team_members.size > 0 %}
{% for member in team_members %}
[{{ member.name | default: member.title }}]({{ member.url | relative_url }})

{% if member.research_focus %}
{{ member.research_focus }}
{% endif %}

{% endfor %}
{% else %}
No team members published yet.
{% endif %}
