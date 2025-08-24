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

{% capture extra %}
{% include publications.md %}
{% endcapture %}
{{ extra | markdownify }}

{% capture extra %}
{% include projects.md %}
{% endcapture %}
{{ extra | markdownify }}

{% capture extra %}
{% include education.md %}
{% endcapture %}
{{ extra | markdownify }}

{% capture extra %}
{% include hobbies.md %}
{% endcapture %}
{{ extra | markdownify }}
