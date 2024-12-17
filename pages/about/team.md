---
permalink: /about/team.html
layout: people
title: DUNE-US S&C Team
---

{% include org_chart.html %}

{% include wbs_list.html %}
{% assign areas = wbs_list | hash_fetch: site.data.orgs | sort_natural: "wbs_no" %}

<h1>Full Team</h1><br>

<div class="container-fluid">
  <div class="row">
     {% for area in areas %}
     {% endfor %}
  </div>
</div>