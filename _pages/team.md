---
layout: page
title: "Team"
permalink: /team/index.html
---

<!-- Jump to [research staff](#research-staff), [PhD students](#phd-students), [PhD alumni](#phd-alumni), [post-doc alumni](#post-doc-alumni). -->

## Professor

{% assign number_printed = 0 %}
{% for member in site.data.team.professor %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row row-buffer">
{% endif %}

<div class="col-sm-6 clearfix column-buffer">
  <img class="img-responsive team-pic" src="{{ site.url }}{{ site.baseurl }}/images/team/individuals/{{ member.photo }}"  />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <a>{{ member.name }}</a>
    {% endif %}
  </h4>
  <br>
  <h5><i>{{ member.role }} </i></h5>

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
{% for member in site.data.team.staff %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row row-buffer">
{% endif %}

<div class="col-sm-6 clearfix column-buffer">
  <img class="img-responsive team-pic" src="{{ site.url }}{{ site.baseurl }}/images/team/individuals/{{ member.photo }}"  />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <a>{{ member.name }}</a>
    {% endif %}
  </h4>
  <br>
  <h5><i>{{ member.role }} </i></h5>

  <ul class="team-info">
  {% if member.info %}
  <li> {{ member.info }} </li>
  {% endif %}
  {% if member.topic %}
  <li> {{ member.topic }} </li>
  {% endif %}
  </ul>

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
{% for member in site.data.team.student %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row row-buffer">
{% endif %}

<div class="col-sm-6 clearfix column-buffer">
  <img class="img-responsive team-pic" src="{{ site.url }}{{ site.baseurl }}/images/team/individuals/{{ member.photo }}"  />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <a>{{ member.name }}</a>
    {% endif %}
  </h4>
  <i>Joined {{ member.joined }} ({{ member.role }}) </i>
  <br>

  <ul class="team-info">
  {% if member.topic %}
  <li> {{ member.topic }}. </li>
  {% endif %}
  {% if member.coadvisor %}
  <li> Co-advised with {{ member.coadvisor }}. </li>
  {% endif %}
  </ul>

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

## PhD Alumni

{% assign number_printed = 0 %}
{% for member in site.data.team.phd-alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row row-buffer">
{% endif %}

<div class="col-sm-6 clearfix column-buffer">
  <img class="img-responsive team-pic" src="{{ site.url }}{{ site.baseurl }}/images/team/individuals/{{ member.photo }}"  />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <a>{{ member.name }}</a>
    {% endif %}
  </h4>
  {% if member.coadvisor %}
    <i>Graduated {{ member.graduated }}, co-advisor {{ member.coadvisor }} </i>
  {% else %}
    <i>Graduated {{ member.graduated }} </i>
  {% endif %}
  <br>

  <ul class="team-info">
  {% if member.thesis-title %}
    {% if member.thesis-link %}
      <li><a href="{{ member.thesis-link }}" target="_blank"> {{ member.thesis-title }}. </a></li>
    {% else %}
      <li><a> {{ member.thesis-title }}. </a></li>
    {% endif %}
  {% endif %}

{% if member.award %}

  <li> {{ member.award }}. </li>
  {% endif %}

{% if member.next %}

  <li> {{ member.next }}. </li>
  {% endif %}
  </ul>

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

## Post-doc Alumni

{% assign number_printed = 0 %}
{% for member in site.data.team.postdoc-alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row row-buffer">
{% endif %}

<div class="col-sm-6 clearfix column-buffer">
  <img class="img-responsive team-pic" src="{{ site.url }}{{ site.baseurl }}/images/team/individuals/{{ member.photo }}"  />
  <h4>
    {% if member.website %}
      <a href="{{ member.website }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <a>{{ member.name }}</a>
    {% endif %}
  </h4>
  {% if member.time-nus %}
    <i> {{ member.role-nus }} at NUS ({{ member.time-nus}}) </i>
  {% else %}
    <i> {{ member.role-nus }} at NUS </i>
  {% endif %}
  <br>

  <ul class="team-info">
  {% if member.phd %}
    <li><a>PhD {{ member.phd }}. </a></li>
  {% endif %}

{% if member.next %}

  <li> {{ member.next }}. </li>
  {% endif %}
  </ul>

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
