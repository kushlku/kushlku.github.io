---
layout: single
author_profile: true
title: ""
hide_title: true
show_recent_posts: false   # hides Recent Posts in sidebar
---

{% capture extra %}
{% include about.md %}
{% endcapture %}
{{ extra | markdownify }}