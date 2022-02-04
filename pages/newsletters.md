---
layout: page
title: Newsletters
url: pages/newsletters/
permalink: newsletters
---


{% assign pdfs = site.static_files | where: "pdf", true %}

{% for pdf in pdfs reversed %}
[{{ pdf.basename }}]( {{ site.url }}/{{ pdf.path }} )
{% endfor %}

