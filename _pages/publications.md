---
permalink: publications/
title: "Publications"
years: [2026,2025, 2024, 2023, 2022]
---


{% for y in page.years %}
  {% bibliography -f references -q @*[year={{y}}]* %}
{% endfor %}
