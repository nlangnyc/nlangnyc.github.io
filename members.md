---
layout: page
title: Blog Ring Members
---

<ul class="memberslist">
{% for member in site.data.members.members %}
  {% assign avatarname = member.github %}
    <li>{% avatar user=avatarname size=128 %}
       <div>
       <h4>{{ member.name }}</h4>
       <br />
       <span class="entypo-github"></span>
       <a href="http://github.com/{{ member.github }}">
       {{ member.github }}</a>
       <br />
       <span class="entypo-rss"></span>
       &nbsp;<a href="{{ member.blog }}">{{ member.blog }}</a>
       </div>
    </li>

  {% endfor %}
</ul>

<hr/>

<p>
Are you a member of NLang-NYC and want to add your name to this list? Submit a pull request to <a href="https://github.com/nlangnyc/nlangnyc.github.io">the repo</a> with a link to your blog.
</p>
