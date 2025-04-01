---
permalink: /students/
title: ""
excerpt: "Students"
redirect_from: 
  - /students.html
---
{% include base_path %}

<div class="grid-container">
     <a href="{{ base_path}}/images/lake-placid-1.png"><img class="group" src="{{ base_path }}/images/lake-placid-1.png" alt="group retreat" /></a>
     <a href="{{ base_path}}/images/lake-placid-2.png"><img class="group" src="{{ base_path }}/images/lake-placid-2.png" alt="group retreat" /></a>
     <a href="{{ base_path}}/images/lake-placid-3.png"><img class="group" src="{{ base_path }}/images/lake-placid-3.png" alt="group retreat" /></a>
     <a href="{{ base_path}}/images/lake-placid-4.png"><img class="group" src="{{ base_path }}/images/lake-placid-4.png" alt="group retreat" /></a>
</div>
<p style="margin-top:10px;">
I'm lucky to work with an amazing group of students, postdocs, and staff. Here we are with friends, collaborators, and alumni at our group off-site in Lake Placid, NY in March 2025.
</p>
<div style="clear:both;" />

<h1>Visitors</h1>
{% assign people = site.data.students | where: "type", "visitor" | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1>Postdocs</h1>
{% assign people = site.data.students | where: "type", "postdoc" | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1>Staff</h1>
{% assign people = site.data.students | where: "type", "software-engineer" | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1> PhD Students</h1>
{% assign people = site.data.students | where: "type", "phd" | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1>Master's Students</h1>
{% assign people = site.data.students | where: "type", "masters" | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1> Undergrad Students </h1>
{% assign people = site.data.students | where: "type", "ugrad"  | sort: "name" %}
<ul>
{% for person in people %}
<li> {{ person.name }} </li>
{% endfor %}
</ul>

<h1>Postdoc Alumni</h1>
{% assign postdoc-alumni = site.data.students | where: "type", "postdoc-alumni" | sort: "year" %}
<ul>
{% for person in postdoc-alumni %}
<li> <div>{% if person.photo %}<a href="{{ person.photo | replace: 'BASE', base_path}}"><img class="alumnus" src="{{ person.photo | replace: 'BASE', base_path }}" alt="{{ person.name }}" /></a>{% endif %}
     <a class="subtle" href="{{ person.url }}">{{ person.name }}</a> (Postdoc {{ person.year }})<br />
     Most recent position: {{ person.position }}</div>
     <div style="clear:both;"></div></li>
{% endfor %}
</ul>

<h1>PhD Alumni</h1>
{% assign phd-alumni = site.data.students | where: "type", "phd-alumni" | sort: "year" %}
<ul>
{% for person in phd-alumni %}
<li> <div>{% if person.photo %}<a href="{{ person.photo | replace: 'BASE', base_path}}"><img class="alumnus" src="{{ person.photo | replace: 'BASE', base_path }}" alt="{{ person.name }}" /></a>{% endif %}
          <a class="subtle" href="{{ person.url }}">{{ person.name }}</a> (PhD {{ person.year }})<br />
     Dissertation: <i><a href="{{ person.thesis_url }}">{{person.thesis}}</a></i><br />
     Most recent position: {{ person.position }}</div>
     <div style="clear:both;"></div></li>
{% endfor %}
</ul>
