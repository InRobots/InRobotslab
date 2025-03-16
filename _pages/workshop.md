---
title: "InRobots - Workshop"
layout: gridlay
excerpt: "Workshop"
sitemap: false
permalink: /workshop/
---

### We are going to organize a workshop on IROS2025: Towards Autonomy and Resiliency of Field Robotics。
Deploying robots in the field without ethical considerations can cause ecological disruption. As we strive towards developing more autonomous and resilient robotic systems, it is imperative to ensure that these advancements do not come at the expense of ecological health. The integration of sustainable practices within resilient robotic systems represents a frontier that must be navigated with caution and foresight. By focusing on energy-efficient designs, eco-friendly material utilization, and strategies for minimizing ecological footprint during deployment, we can pave the way for a harmonious coexistence between robotics and the natural world.

The intersection of AI and robotics holds great promise for sustainable field deployment, aiming at minimize environmental impact while optimizing resource use across multiple domains, such as agricultural automation, environmental monitoring, disaster response, and mining. In light of this, bringing together experts from academia and industry, we aim to address scientific and technical questions such as: How can AI-powered robots enhance ecological sustainability in field applications? What materials and designs are most conducive to reducing the environmental impact of robotic systems? How can we trade off the resiliency in swarm robotics and potential increase in material usage? By fostering interdisciplinary dialogue and innovation, our workshop seeks to contribute to the development of robotic systems that are not only technologically advanced but also environmentally responsible. 

## Organizers
{% assign number_printed = 0 %}
{% for member in site.data.workshop %}

{% assign even_odd = number_printed | modulo: 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/workshop/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  {% if member.number_info == 1 %}
  <li> {{ member.information }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
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


## Keynote Speakers

{% assign number_printed = 0 %}
{% for member in site.data.keynote %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/keynote/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <br> {{ member.apt }}</i>
  <!--<i>{{ member.duration }} <br> Role: {{ member.info }}</i>-->
  <ul style="overflow: hidden">

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
