{% assign publications = site.publications | sort: "date" | reverse %}
{% for publication in publications %}
- **{{ publication.title }}** \\
	{{ publication.authors }} \\
	_{{ publication.venue}}_, {{ publication.location }}. \\
	{{ publication.date | date: "%B %Y" }} \\
	{{ publication.notes }} \\
	{{ publication.content | markdownify }}
{% endfor %}
