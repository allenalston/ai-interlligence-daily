---
layout: home
title: 最新日报列表
---

# 📅 历史日报存档 (按时间倒序)

<ul>
{% assign sorted_pages = site.pages | sort: 'path' | reversed %}
{% for file in sorted_pages %}
  {% if file.path contains 'news/' %}
    <li><a href="{{ site.baseurl }}{{ file.url }}">{{ file.name | replace: ".md", "" }}</a></li>
  {% endif %}
{% endfor %}
</ul>

---
*提示：以上列表由 Jekyll 自动根据文件名倒序生成。*
