---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  这里是网站架构说明书 <span style="font-weight: bold">[[Your first note]]</span> ，没啥用。
</p>


还没想好主页的样式，你看到这里，说明BIANO的小站搭建成功了。

这是我2017年至今找到的[[看书记录]]

这是看过的书汇总列表[[书库]]

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>   

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
