{% assign presentations = site.presentations | sort: "date" | reverse %}
{% for presentation in presentations %}
- **{{ presentation.title }}** \\
	{{ presentation.authors }} \\
	_{{ presentation.venue}}_, {{ presentation.location }}. \\
	{{ presentation.date | date: "%d.%m.%Y" }} \\
	{{ presentation.notes }} \\
	{{ presentation.content | markdownify }}
{% endfor %}