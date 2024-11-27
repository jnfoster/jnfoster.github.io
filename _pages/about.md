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

# News

<ul>
{% for item in site.data.news %}
{% if item.type == "cond_acceptance" %}
<li>[{{item.month}}/{{item.year}}] <b>{{ item.name }}</b> conditionally accepted to <a href="{{ item.conference_url }}">{{ item.conference }}</a>.</li>
{% endif %}
{% if item.type == "acceptance" %}
<li>[{{item.month}}/{{item.year}}] <b>{{ item.name }}</b> accepted to <a href="{{ item.conference_url }}">{{ item.conference }}</a>.</li>
{% endif %}
{% if item.type == "award" %}
<li>[{{item.month}}/{{item.year}}] <b>{{ item.description}}</b> from <a href="{{ item.url }}">{{ item.organization }}</a>.</li>
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
<a class="file_link paper" href="{{ base_path }}/papers/p4cub.pdf">CPP '23</a>
<a class="file_link paper" href="{{ base_path }}/papers/leapfrog.pdf">PLDI '22</a><br />
<a class="file_link paper" href="{{ base_path }}/papers/petr4.pdf">POPL '21</a>
<a class="file_link code" href="https://github.com/cornell-netlab/petr4/">Code</a>
</div>
</div>
<div class="container">
<div class="box-6 feature">
<img src="images/pronto-logo.png" alt="Pronto logo" /><br />
Verifiable Closed-Loop Control for Next-Generation Networks<br />
<a class="file_link paper" href="{{ base_path }}/papers/formal-scheduling.pdf">OOPSLA '23</a>
<a class="file_link paper" href="{{ base_path }}/papers/hydra.pdf">SIGCOMM '23</a><br />
<a class="file_link paper" href="{{ base_path }}/papers/pronto-ccr.pdf">CCR '20</a>
<a class="file_link paper" href="{{ base_path }}/papers/avenir.pdf">NSDI '21</a>
</div>
<div class="box-6 feature">
<img src="images/netkat-logo.png" alt="NetKAT logo" /><br />
(Co)-Algebraic Foundations for Programmable Networks<br />
<a class="file_link paper" href="{{ base_path }}/papers/mcnetkat.pdf">PLDI '19</a>
<a class="file_link paper" href="{{ base_path }}/papers/gkat.pdf">POPL '20</a>
</div>
</div>
<div class="container">
<div class="box-6 feature">
<img src="images/neptune-logo.png" alt="Neptune logo" /><br />
Flexibility, Performance, Consistency for Heterogeneous Packet-Processing Architectures<br />
<a class="file_link webpage" href="https://www.cs.cornell.edu/information/news/newsitem11102/multiple-google-faculty-research-awards-cornell-cs-including-nate">CS article</a>
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

[npi]: https://network-programming.org
