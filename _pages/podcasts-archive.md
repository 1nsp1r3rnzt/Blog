---
permalink: /podcasts/
layout: collection
author_profile: true
title: "Fav. Podcast's Notes"
entries_layout: grid
classes: wide
collection: podcasts
show_content: after
---
<div><h2>Recent Podcasts Notes
</h2></div>
{% assign sorted = site.podcastepisodes | sort: 'date' | reverse %}
{% for post in sorted limit:5 %}
{% include archive-single.html show_podcast_title="true" %}
{% endfor %}
<a href="/podcasts-archive/">All Podcasts Archive</a>