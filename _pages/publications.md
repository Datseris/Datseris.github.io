---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

*remember that you can always ask me for pdf versions of any paper I
have written, and I'd gladly share*

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
