---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

My papers are also listed on [Google Scholar]({{ site.author.googlescholar }}) and [ORCID]({{ site.author.orcid }}).

<h2 class="archive__subtitle">Journal Articles</h2>

{% assign journal_articles = site.publications | where: "pub_type", "journal" | sort: "date" | reverse %}
{% for post in journal_articles %}
  {% include archive-single.html %}
{% endfor %}

<h2 class="archive__subtitle">Conference Papers</h2>

{% assign conference_papers = site.publications | where: "pub_type", "conference" | sort: "date" | reverse %}
{% for post in conference_papers %}
  {% include archive-single.html %}
{% endfor %}
