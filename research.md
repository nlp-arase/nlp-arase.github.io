---
layout: page
title : Research
permalink: /research/
---

<h3 class="member-role"><span>研究内容</span></h3>
<div class="member-content">
{% for UT in site.data.research %}
    <span>{{ UT.UpperTheme }}</span>
    {% for LT in UT.LowerTheme %}
        <div class="research-theme">{{ LT.theme }}</div><BR>
        <div class="research-content">{{ LT.contents }}</div>
    {% endfor %}
{% endfor %}
</div>