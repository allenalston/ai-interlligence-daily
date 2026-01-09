---
layout: home
title: 最新日报列表
---

# 📅 历史日报存档

{% for file in site.static_files %}
  {% if file.path contains 'daily-reports/' %}
    * [{{ file.basename }}]({{ file.path }})
  {% endif %}
{% endfor %}

---
*提示：以上列表由 Jekyll 自动根据文件夹内容生成。*
