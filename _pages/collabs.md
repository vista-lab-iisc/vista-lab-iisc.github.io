---
layout: default
title: Collaborations
permalink: /collaborations2/
---

# {{ page.title }}

## Industry Collaborations
<div style="display: flex; flex-wrap: wrap;">
<!-- <div class="col-sm-6 clearfix"> -->
{% for collaboration in site.data.industry_collab %}
  <div style="flex: 1 0 24%; margin: 1%; box-sizing: border-box;">
    <figure>
      <img src="{{ site.url }}{{ site.baseurl }}/images/collab/{{ collaboration.logo }}" alt="{{ collaboration.name }}" style="width: 100%; height: auto;">
      <!-- <figcaption>{{ collaboration.name }}</figcaption> -->
    </figure>
  </div>
{% endfor %}
</div>

## Government Collaborations
<div style="display: flex; flex-wrap: wrap;">
{% for collaboration in site.data.government_collaborations %}
  <div style="flex: 1 0 24%; margin: 1%; box-sizing: border-box;">
    <figure>
      <img src="{{ site.url }}{{ site.baseurl }}/images/collaboration/{{ collaboration.logo }}" alt="{{ collaboration.name }}" style="width: 100%; height: auto;">
      <figcaption>{{ collaboration.name }}</figcaption>
    </figure>
  </div>
{% endfor %}
</div>

## University Collaborations
<div style="display: flex; flex-wrap: wrap;">
{% for collaboration in site.data.university_collaborations %}
  <div style="flex: 1 0 24%; margin: 1%; box-sizing: border-box;">
    <figure>
      <img src="{{ site.url }}{{ site.baseurl }}/images/collaboration/{{ collaboration.logo }}" alt="{{ collaboration.name }}" style="width: 100%; height: auto;">
      <figcaption>{{ collaboration.name }}</figcaption>
    </figure>
  </div>
{% endfor %}
</div>
