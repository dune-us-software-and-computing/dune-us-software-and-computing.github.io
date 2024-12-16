---
layout: main-page
title: Home
<!--- bgimage: assets/images/USCMS_banner.png --->
---

# Mission

The mission of DUNE-US Software and Computing is to provide the computing resources necessary to process DUNE data efficiently, and to develop core software in support of the data analysis efforts of the international DUNE collaboration to enable discovery physics, in collaboration with international DUNE Software and Computing partners.


# Areas
DUNE-US Software and Computing is broken down into four areas:


{% assign areas = site.pages | where: "layout", "wbs-area" | sort_natural: 'wbs_no' %}
{% for mypage in areas %}
- [{{mypage.title}} (WBS {{mypage.wbs_no}})]({{mypage.permalink}})
{% endfor %}
