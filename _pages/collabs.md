---
layout: default
title: Collaborations
---

# {{ page.title }}

## Industry Collaborations
{% for collaboration in site.data.industry_collab %}
### {{ collaboration.name }}
![{{ collaboration.name }}]({{ site.url }}{{ site.baseurl }}/images/collaboration/{{ collaboration.logo }})
{% endfor %}

## Government Collaborations
{% for collaboration in site.data.government_collaborations %}
### {{ collaboration.name }}
![{{ collaboration.name }}]({{ site.url }}{{ site.baseurl }}/images/collaboration/{{ collaboration.logo }})
{% endfor %}

## University Collaborations
{% for collaboration in site.data.university_collaborations %}
### {{ collaboration.name }}
![{{ collaboration.name }}]({{ site.url }}{{ site.baseurl }}/images/collaboration/{{ collaboration.logo }})
{% endfor %}
