---
layout: page
title: Home
id: home
permalink: /
---

# Hi, I'm Chandu Avni! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Digital Garden Guiding Principles]]</span> to get started on your exploration.
</p>

Welcome to my digital garden! This is a place where I can share my learnings and grow my thoughts.

Learn more [about me](/about) or visit my [main website](https://chanduavni.com/).

<strong>Recently Updated Notes</strong>

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
