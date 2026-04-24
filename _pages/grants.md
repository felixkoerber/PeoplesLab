---
title: Grants
subtitle: Funded research lines and collaborations
description: Overview of current and past grants
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
