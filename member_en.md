---
layout: page
title: Member
permalink: /en/member/
anotherlink: /member/
category: "member"
tagline: "Arase Group Member"
lang: en
---

<h3 class="member-role"><span>Professors</span></h3> 

{% for person in site.data.professors %}
  <ul class="member-content">
    {{ person.name_en }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}

<h3 class="member-role"><span>Students</span></h3>

{% for person in site.data.students %}
  <ul class="member-content">
    {{ person.name_en }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}
