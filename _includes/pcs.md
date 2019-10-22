{% assign pcs = site.pcs | sort: "date" | reverse %}
{% for pc in pcs %}
- **{{ pc.title }}** \\
	_{{ pc.long_title }}_ \\
	{{ pc.location }}. \\
	{{ pc.role}}
{% endfor %}