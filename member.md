---
layout: page
title: メンバー
permalink: /member/
anotherlink: /en/member/
category: "member"
tagline: "荒瀬班の愉快な仲間たち"
lang: ja
---

<h3 class="member-role"><span>Professors</span></h3> 

{% for person in site.data.professors %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {% for link in person.introduction %}
        <a target='_blank' rel='noopener noreferrer' href='{{ link.link }}'>{{ link.name }}</a> /
    {% endfor %}
  </ul>
{% endfor %}

<h3 class="member-role"><span>Students</span></h3>

{% for person in site.data.students %}
  <ul class="member-content">
    {{ person.name }} | {{ person.grade }} <br>
    {% for link in person.introduction %}
        <a target='_blank' rel='noopener noreferrer' href='{{ link.link }}'>{{ link.name }}</a> /
    {% endfor %}
  </ul>
{% endfor %}
