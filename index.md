---
layout: home
title: AI 行业情报站
---

# 📅 历史日报存档

{% for file in site.static_files %}
  {% if file.path contains 'daily-reports/' %}
    * [{{ file.basename }}]({{ file.path }})
  {% endif %}
{% endfor %}
