---
title: "VISTA Lab - Team"
layout: gridlay
excerpt: "VISTA Lab: Team members"
sitemap: false
permalink: /team/
---

 <!-- **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** -->


## Lab Head
{% assign number_printed = 0 %}
{% for member in site.data.lab_head %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
  Research Domains:<br /> {{ member.domains }}<br/>
  <div class="member-links">
  <a href="{{ member.linkedin }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/iisc.png" alt="LinkedIn" class="icon">
  </a>
  <a href="{{ member.google_scholar }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/iisc.png" alt="Scholar" class="icon">
  </a>
  </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Research Staff
{% assign number_printed = 0 %}
{% for member in site.data.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
  Research Domains:<br /> {{ member.domains }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.phd_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
  Research Domains:<br /> {{ member.domains }}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Master Students

{% for member in site.data.mtech_students %} <br>{{ member.name }}<br /> {% endfor %}

## Interns

<style>
  .icon {
    width: 24px; /* or any desired size */
    height: auto;
    margin-right: 8px; /* add some space between icons */
    transition: transform 0.3s ease; /* optional: for hover effect */
  }

  .icon:hover {
    transform: scale(1.1); /* optional: for hover effect */
}

</style>

<!-- ## Alumni

## Former visitors

## Administrative Support -->