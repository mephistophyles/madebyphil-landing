---
title: "LLM sourced MBA curriculum"
layout: default
date: 2025-04-04
permalink: /llm-mba/
---

# {{ page.title }}

I've started to build out a comprehensive MBA curriculum with a number of LLM tools. It's hard to validate it for completeness or if it's as comprehensive as it needs to be. So for now my plan is to go through it as I'm learning the material, with a skeptical eye, and update the content here. Feel free to suggest edits in the github repo or by emailing me.

<ul>
  {% assign parent_url = page.url %}
  {% for child in site.pages %}
    <li>{{ child.url }} - {{parent_url}} - </li>
    {% if child.url != page.url and child.url contains parent_url %}
      {%- assign relative_path = child.url | remove: parent_url -%}
      {%- assign segments = relative_path | split: '/' -%}
      {% if segments.size == 1 or (segments.size == 2 and segments[1] == "") %}
        <li><a href="{{ child.url }}">{{ child.title }}</a></li>
      {% endif %}
    {% endif %}
  {% endfor %}
</ul>