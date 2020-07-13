---
title: 'Machine Learning and Vision Group - Team'
layout: gridlay
excerpt: 'Team members'
sitemap: false
permalink: /team/
---

### Phd Students

{% assign number_printed = 0 %}
{% for member in site.data.current_students.phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.webpage.size > 0 %}
  <h4><a href='{{ member.webpage }}' target='_blank'>{{ member.name }}</a></h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}

<i>{{ member.desig }}</i> <br/>
<i>{{ member.info }}<br/>
ID: {{ member.id }}</i>

  <!-- email, gscholar -->
  <div class="" style="display: flex">
  {% if member.email.size > 0 %}
  <a href="mailto: {{member.email}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="fa fa-envelope"></i></a>
  {% endif %}
  {% if member.google-scholar.size > 0 %}
  <a href="{{member.google-scholar}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="ai ai-google-scholar-square ai-3x"></i></a>
  {% endif %}
  </div>
  
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
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

### Masters Students

{% assign number_printed = 0 %}
{% for member in site.data.current_students.masters %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.webpage.size > 0 %}
  <h4><a href='{{ member.webpage }}' target='_blank'>{{ member.name }}</a></h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}
  <i>{{ member.desig }}</i> <br/>
  <i>{{ member.info }}<br/>
  ID: {{ member.id }}</i> 
  <div class="" style="display: flex">
  {% if member.email.size > 0 %}
  <a href="mailto: {{member.email}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="fa fa-envelope"></i></a>
  {% endif %}
  {% if member.google-scholar.size > 0 %}
  <a href="{{member.google-scholar}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="ai ai-google-scholar-square ai-3x"></i></a>
  {% endif %}
  </div>
  
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
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

### Research Assistants/Interns

{% assign number_printed = 0 %}
{% for member in site.data.current_students.third_party_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.webpage.size > 0 %}
  <h4><a href='{{ member.webpage }}' target='_blank'>{{ member.name }}</a></h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}
  <!-- <i>{{ member.desig }}</i> <br/> -->
  <i>{{ member.info }}<br/>
  ID: {{ member.id }}</i> 
  <div class="" style="display: flex">
  {% if member.email.size > 0 %}
  <a href="mailto: {{member.email}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="fa fa-envelope"></i></a>
  {% endif %}
  {% if member.google-scholar.size > 0 %}
  <a href="{{member.google-scholar}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="ai ai-google-scholar-square ai-3x"></i></a>
  {% endif %}
  </div>
  
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
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

### Undergrad Students

{% assign number_printed = 0 %}
{% for member in site.data.current_students.undergrad %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}

<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% if member.webpage.size > 0 %}
  <h4><a href='{{ member.webpage }}' target='_blank'>{{ member.name }}</a></h4>
  {% else %}
  <h4>{{ member.name }}</h4>
  {% endif %}
  <i>{{ member.desig }}</i> <br/>
  <i>{{ member.info }}<br/>
  ID: {{ member.id }}</i> 
  <div class="" style="display: flex">
  {% if member.email.size > 0 %}
  <a href="mailto: {{member.email}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="fa fa-envelope"></i></a>
  {% endif %}
  {% if member.google-scholar.size > 0 %}
  <a href="{{member.google-scholar}}" target="_blank"><i style="font-size: 30px; margin-right: 10px;" class="ai ai-google-scholar-square ai-3x"></i></a>
  {% endif %}
  </div>
  
  <ul style="overflow: hidden">
  
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
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
