---
layout: default
title: CLunch Archive
order: 3
---
# CLunch Archive
Here are the past talks given at CLunch.

{% assign talks_size = site.data.clunch_archive | size %}
{% if talks_size > 0 %}
  <p>
  <h2>CLunch Archive</h2>

  {% for talk in site.data.clunch_archive %}
    {% include talk.html speaker=talk.speaker img=talk.img url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
{% endif %}
