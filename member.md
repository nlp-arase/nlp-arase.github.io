---
layout: page
title: Member
permalink: /member/
category: "member"
tagline: "荒瀬班の愉快な仲間たち"
---


{% for person in site.data.member %}
  <li class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {{ person.introduction }}
  </li>
{% endfor %}
