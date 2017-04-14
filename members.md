---
layout: page
title: Members 
---

<ul>
{% for member in site.data.members.members %}
 <li>{{ member.name }} 
     <em>@<a href="http://github.com/{{ member.github }}">{{ member.github }}</a></em>
     <br />
     <a href="{{ member.blog }}">{{ member.blog }}</a>
 </li>
{% endfor %}
</ul>
