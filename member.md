---
layout: page
title: Member
permalink: /member/
category: "member"
tagline: "荒瀬班の愉快な仲間たち"
lang: ja
---
Japanese
<h3 class="member-role"><span>Professors</span></h3> 

{% for person in site.data.professors %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}

<h3 class="member-role"><span>Students</span></h3>

{% for person in site.data.students %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </ul>
{% endfor %}
