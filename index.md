---
layout: homepage
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
{% include timeline.md %}
{% endcapture %}
{{ extra | markdownify }}

{% capture extra %}
{% include hobbies.md %}
{% endcapture %}
{{ extra | markdownify }}
