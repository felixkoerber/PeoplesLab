---
title: Grants
description: A list of current Grants awarded to the People's Lab
permalink: /grants
---

<section class="portfolio">
	<section class="single">
		{% for grant in site.grants reversed %}
		<h2><a href="{{ grant.url | relative_url }}">{{ grant.project_name | default: grant.title }}</a></h2>
		{% if grant.Applicant %}<p><strong>Applicant:</strong> {{ grant.Applicant }}</p>{% endif %}
		{% if grant.Term %}<p><strong>Term:</strong> {{ grant.Term }}</p>{% endif %}
		<hr>
		{% endfor %}
	</section>
</section>
