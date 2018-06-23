---
layout: archive
title: "Podcast Archive"
permalink: /podcasts-archive/
author_profile: true
---
<a href="/podcasts/" class="archive__subtitle">View by Category</a>
    {% assign sorted = site.podcastepisodes | sort: 'date' | reverse %}

  {% for post in sorted %}

{% include archive-single.html show_podcast_title="true" %}

  {% endfor %}


  