---
layout: default
title: CLunch
order: 3
---
# CLunch
CLunch is the weekly <b>c</b>omputational linguistics <b>lunch</b> run by the NLP group.
We invite external and internal speakers to come and present their research on natural language processing, computational linguistics, and machine learning.

Interested in attending CLunch? Sign up for our mailing list [here](http://lists.seas.upenn.edu/mailman/listinfo/clunch).

{% assign talks_size = site.data.clunch | size %}
{% if talks_size > 0 %}
  <p>
  <h2>Talks</h2>

  {% for talk in site.data.clunch %}
    {% include talk.html speaker=talk.speaker url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
{% endif %}
