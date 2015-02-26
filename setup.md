---
layout: archive
permalink: /setup/
title: 建站
---

<div class="tiles">
{% for post in site.categories.setup%}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
