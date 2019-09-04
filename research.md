---
layout: page
title : 研究内容
permalink: /research/
anotherlink: /en/research/
category: "research"
tagline: "取り組んでいる分野と研究を紹介します．"
lang: ja
---

<div>
{% for UT in site.data.research %}
    <h3 class="member-role"><span>{{ UT.UpperTheme }}</span></h3>
    {% for LT in UT.LowerTheme %}
        <div class="research-area">
            <div class="research-theme">{{ LT.theme }}</div><BR>
            <div class="research-content">{{ LT.contents }}</div>
            {% for image in LT.img %}
                <div class="research-img" style="background: url({{ site.baseurl }}/image/{{ image }})"></div>
            {% endfor %}
        </div>
    {% endfor %}
{% endfor %}
</div>