---
title: "Blog"
permalink: /blog/
layout: single
author_profile: true
excerpt_separator: <!--more-->
classes: wide
---

<ul>
  {% for post in site.posts %}
    <li style="list-style-type: none;">
      &#10084; <a href="{{ post.url }}" style="text-transform: uppercase;"> {{ post.title }}</a>
      <p style="margin-left:10px; font-size:12pt">&#128214; <b>Published:</b> {{ post.date | date: "%-d %B %Y"}} </p>
      <p style="margin-left:30px;font-size:11pt;">{{ post.content | strip_html | truncatewords: 50 }}</p>
    </li>
  {% endfor %}
</ul>