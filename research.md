---
layout: page
title : Research
permalink: /ja/research/
category: "research"
---

<h2>研究内容</h2>
{% for UpperTheme in site.data.research %}
    <div class="manual-post">
        <div class="manual manual-title">
            <strong>{{ UpperTheme.UpperTheme }}</strong>
        </div>
    {% for LowerTheme in UpperTheme.LowerTheme %}
        <div class="manual-content">
            <span class='manual'>{{ LowerTheme.theme }}</span><BR>
            <pre>---
            {{ LowerTheme.contents }}
            \---</pre>
        </div>
    {% endfor %}
    </div>
{% endfor %}
