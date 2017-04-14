---
layout: page
title: Members 
---

<ul class="memberslist">
{% for member in site.data.members.members %}
  {% assign avatarname = member.github %}
    <li>{% avatar user=avatarname size=128 %}
       {{ member.name }} 
       <br />
       <em>@<a href="http://github.com/{{ member.github }}">{{ member.github }}</a></em>
       <br />
       <a href="{{ member.blog }}">{{ member.blog }}</a>
    </li>
  {% endfor %}
</ul>
