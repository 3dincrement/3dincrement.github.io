---
layout: team
title: Team
description: 团队成员
keywords: 团队成员, Member
comments: false
menu: 团队
permalink: /member/
---

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 ">
<div class="row">
	<div class="col-sm-3 col-sm-push-1 center-block"><br>
		<a href="{{ site.url }}{{ site.baseurl }}/member/{{ member.name }}"  >	
		<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class=" img-responsive img-rounded"/></a>
	</div>
	<div class="col-sm-8 col-sm-push-1">
	  <h4>{{ member.name }}</h4>
	  <i>{{ member.info }}
	  <br>email: <a href="{{ member.email }}">{{ member.email }}</a><br>github: <a href="{{ member.github }}">{{ member.github }}</a></i>
	</div>
</div>
<br>
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
