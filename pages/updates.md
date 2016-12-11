---
layout: page
title: Updates
permalink: /updates/
slider: true
heading: Get The Latest On What We're Doing!
subheading: Catch up with us, anytime, anywhere
---

{% for post in site.posts %}
<div class="post-area">
  <a href="{{ post.url | prepend: site.baseurl }}" class="bold">{{ post.title }}</a>
  <p class="post-date">{{ post.date | date_to_long_string }}</p>
  <p>
    {{ post.content | strip_html | truncatewords: 50 }}
  </p>
</div>
{% endfor %}
