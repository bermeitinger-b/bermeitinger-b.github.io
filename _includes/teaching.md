{% assign courses = site.teaching | sort_natural: "semester" | reverse %}
{% for course in courses %}
- **{{ course.title }}** \\
	_{{ course.location}}_. \\
	{{ course.semester }} \\
	{{ course.role }}
{% endfor %}