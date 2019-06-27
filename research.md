---
layout: page
title : Research
permalink: /research/
---

<h2>研究内容</h2>
{% for UT in site.data.research %}
    <div class="manual-post">
        <div class="manual manual-title">
            <strong>{{ UT.UpperTheme }}</strong>
        </div>
    {% for LT in UT.LowerTheme %}
        <div class="manual-content">
            <span class="manual">{{ LT.theme }}</span><BR>
            <pre>{{ LowerTheme.contents }}</pre>
        </div>
    {% endfor %}
    </div>
{% endfor %}
