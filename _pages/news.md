---
permalink: /news/
title: "News"
excerpt: "News"
author_profile: false
redirect_from: 
  - /news.html
---

{% include base_path %}

<ul>
{% for item in site.data.news %}
{% if item.type == "announce" %}
<li>[{{item.month}}/{{item.year}}] {{ item.description }}.</li>
{% endif %}
{% if item.type == "cond_acceptance" %}
<li>[{{item.month}}/{{item.year}}] <i>{{ item.name }}</i> conditionally accepted to <a class="subtle" href="{{ item.conference_url }}">{{ item.conference }}</a>.</li>
{% endif %}
{% if item.type == "acceptance" %}
<li>[{{item.month}}/{{item.year}}] <i>{{ item.name }}</i> accepted to <a class="subtle" href="{{ item.conference_url }}">{{ item.conference }}</a>.</li>
{% endif %}
{% if item.type == "award" %}
<li>[{{item.month}}/{{item.year}}] {{ item.description}} from <a class="subtle" href="{{ item.url }}">{{ item.organization }}</a>.</li>
{% endif %}
{% endfor %}
</ul>

