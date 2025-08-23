---
permalink: /
title: "Home"
excerpt: "Home"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

My research uses ideas from programming languages to solve problems in
networking, databases, and security. Some specific topics of interest
include language design, semantics, type systems, and mechanized
proof. Recently I've been spending most of my time thinking about how
to design better languages and tools for computer networks.

# Recent News [<a href="{{ base_path }}/news">all</a>]

<ul>
{% for item in site.data.news limit:7 %}
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

# Current Projects

<div class="container">
<div class="box-6 feature">
<img src="images/lancer-logo.png" alt="LANCER logo" /><br />
Reinforcement Learning for Network Security<br />
<a class="file_link webpage" href="https://news.cornell.edu/stories/2023/10/computer-scientists-awarded-3m-bolster-cybersecurity">Chronicle article</a>
</div>
<div class="box-6 feature">
<img src="images/petr4-logo.png" alt="Petr4 logo" /><br />
Formal Foundations for Programmable Data Planes<br />
<a class="file_link paper" href="{{ base_path }}/papers/p4testgen.pdf">SIGCOMM '24a</a>
<a class="file_link paper" href="{{ base_path }}/papers/hydra.pdf">SIGCOMM '24b</a>
<a class="file_link paper" href="{{ base_path }}/papers/p4cub.pdf">CPP '23</a>
<a class="file_link paper" href="{{ base_path }}/papers/leapfrog.pdf">PLDI '22</a><br />
<a class="file_link paper" href="{{ base_path }}/papers/petr4.pdf">POPL '21</a>
<a class="file_link code" href="https://github.com/cornell-netlab/petr4/">Code</a>
</div>
</div>
<div class="container">
<div class="box-6 feature">
<img src="images/netkat-logo.png" alt="NetKAT logo" /><br />
(Co)-Algebraic Foundations for Programmable Networks<br />
<a class="file_link webpage" href="https://netkat.org">Project webpage</a>
<a class="file_link paper" href="{{ base_path }}/papers/katch.pdf">PLDI '24</a>
<a class="file_link paper" href="{{ base_path }}/papers/mcnetkat.pdf">PLDI '19</a>
<a class="file_link paper" href="{{ base_path }}/papers/gkat.pdf">POPL '20</a>
</div>
<div class="box-6 feature">
<img src="images/littleton-logo.png" alt="Littleton logo" /><br />
A Programming Language for Future Interests<br />
<a class="file_link webpage" href="https://conveyanc.es/">Webpage</a>
<a class="file_link paper" href="{{ base_path }}/papers/conveyances-yjolt.pdf">YJoLT '22</a><br />
<a class="file_link paper" href="{{ base_path }}/papers/conveyances.pdf">Onward! '19</a>
</div>
</div>
<br />
