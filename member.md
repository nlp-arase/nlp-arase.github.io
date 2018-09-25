---
layout: page
title: Member
permalink: /member/
category: "member"
tagline: "荒瀬班の愉快な仲間たち"
---

<h3 class="member-role"><a>Professors</a></h3> 

{% for person in site.data.professors %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}

<h3 class="member-role"><a>Students</a></h3>

{% for person in site.data.students %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}
