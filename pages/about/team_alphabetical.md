---
permalink: /about/team_alphabetical.html
layout: people
title: Institute Team
---

{% include org_chart.html %}

{% include institution_list.html %}
{% assign members = site.data.people | values
                                     | where_exp:"item", "item.active and item.hidden != true"
                                     | last_name_sort: "name" %}
{% assign former_members = site.data.people | values
                                    | where_exp:"item", "item.active == false and item.hidden != true"
                                    | last_name_sort: "name" %}


<h1>Full Team</h1><br>

<div class="container-fluid">
<div class="row">
</div>
</div>
