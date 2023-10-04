---
title: "VISTA Lab - Team"
layout: gridlay
excerpt: "VISTA Lab: Team members"
sitemap: false
permalink: /team/
---

 <!-- **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** -->


### Lab Head
{% assign number_printed = 0 %}
{% for member in site.data.lab_head %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<!-- <div class="col-sm-6 clearfix"> -->
<div class="col-sm-12 clearfix"> <!-- Changed from col-sm-6 to col-sm-12 -->
  <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> -->
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive member-img" alt="{{ member.name }}"/>
  <h4><y>{{ member.name }}</y></h4>
  <i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
  Research Interests: {{ member.domains }}<br/>
  <!-- <div class="member-links"> -->
  <a href="{{ member.website }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/website.png" alt="Website" class="icon">
  </a>
  <a href="{{ member.linkedin }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/linkedin.png" alt="LinkedIn" class="icon">
  </a>
  <a href="{{ member.google_scholar }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/google.png" alt="Scholar" class="icon">
  </a>
  <a href="{{ member.github }}" target="_blank">
  <img src="{{ site.url }}{{ site.baseurl }}/images/icons/github.png" alt="GitHub" class="icon">
  </a>
  <!-- </div> -->
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

<br/>

### Research Staff
{% for member in site.data.staff %}
<div class="row">
<div class="col-sm-12 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive member-img" alt="{{ member.name }}"/>
<h4><y>{{ member.name }}</y></h4>
<i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
Research Interests: {{ member.domains }}<br/>
<a href="{{ member.linkedin }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/linkedin.png" alt="LinkedIn" class="icon">
</a>
<a href="{{ member.google_scholar }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/google.png" alt="Scholar" class="icon">
</a>
<a href="{{ member.github }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/github.png" alt="GitHub" class="icon">
</a>
</div>
</div>
{% endfor %}
<br/>

### PhD Students
{% for member in site.data.phd_students %}

<div class="row">
<div class="col-sm-12 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive member-img" alt="{{ member.name }}">
<h4><y>{{ member.name }}</y></h4>
<i>{{ member.info }} <br>email: <{{ member.email }}></i><br />
Research Interests: {{ member.domains }}<br/>
<a href="{{ member.linkedin }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/linkedin.png" alt="LinkedIn" class="icon">
</a>
<a href="{{ member.google_scholar }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/google.png" alt="Scholar" class="icon">
</a>
<a href="{{ member.github }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/github.png" alt="GitHub" class="icon">
</a>
</div>
</div>

{% endfor %}

<br/>

### Master Students

{% for member in site.data.mtech_students %}

<div class="row">
<div class="col-sm-12 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive member-img" alt="{{ member.name }}">
<h4><y>{{ member.name }}</y></h4>
{{ member.info }} <br>email: {{ member.email }}<br />
Research Interests: {{ member.domains }}<br/>
<a href="{{ member.linkedin }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/linkedin.png" alt="LinkedIn" class="icon">
</a>
<a href="{{ member.google_scholar }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/google.png" alt="Scholar" class="icon">
</a>
<a href="{{ member.github }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/icons/github.png" alt="GitHub" class="icon">
</a>
</div>
</div>

{% endfor %}

<br/>

<br/>
### Interns

<style>
  .icon {
    width: 26px; /* or any desired size */
    height: auto;
    margin-right: 8px !important; /* add some space between icons */
    transition: transform 0.3s ease; /* optional: for hover effect */
    box-shadow: none !important; /* Removes shadow */
  }

  .member-img {
    width: 150px; /* Or any desired size */
    height: 150px; /* Should be the same as width for a square image */
    object-fit: cover;
    float: left;
  }

  .icon-link {
    display: inline-block; /* or you can use 'inline' */
    /* white-space: nowrap; */
    /* margin-right: 5px; Optional: for some spacing between the icons */
  }

  .icon-container {
    white-space: nowrap;
  }

  /* .icon:hover { */
    /* transform: scale(1.1); optional: for hover effect */
/* } */

</style>

<!-- ## Alumni

## Former visitors

## Administrative Support -->