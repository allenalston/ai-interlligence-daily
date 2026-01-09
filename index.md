---
layout: home
title: 最新日报列表
---

# 📅 历史日报存档

<ul>
{% for file in site.pages %}
  {% if file.path contains 'daily-reports/' %}
    <li><a href="{{ site.baseurl }}{{ file.url }}">{{ file.name | replace: ".md", "" }}</a></li>
  {% endif %}
{% endfor %}
</ul>

---
*提示：以上列表由 Jekyll 自动根据文件夹内容生成。*
