{% assign pcs = site.pcs | sort: "date" | reverse %}
{% for pc in pcs %}
- **{{ pc.title }}** \\
	_{{ pc.long_title }}_ \\
	{{ pc.location }}. \\
        {{ pc.date | date: "%B %Y"}} \\
	{{ pc.role}}
{% endfor %}
