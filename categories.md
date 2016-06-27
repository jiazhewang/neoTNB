---
layout: page
title: 文章分类 | Categories
tagline: 分类
---

<ul>
    {% for category in site.categories %}
    <li><a href="/{{ category | first }}/" title="view all
posts">{{ category | first }} {{ category | last | size }}</a>
    </li>
    {% endfor %}
</ul>