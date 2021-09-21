---
layout: default
title: CLunch
order: 3
---
# CLunch
CLunch is the weekly <b>c</b>omputational <b>l</b>inguistics l<b>unch</b> run by the NLP group.
We invite external and internal speakers to come and present their research on natural language processing, computational linguistics, and machine learning.

Interested in attending CLunch? Sign up for our mailing list [here](http://lists.seas.upenn.edu/mailman/listinfo/clunch).

{% assign future_talks_size = site.data.future_clunch | size %}
{% if future_talks_size > 0 %}
  <p>
  <h2>Upcoming Talks</h2>

  {% for talk in site.data.future_clunch %}
    {% include talk.html speaker=talk.speaker url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
  <hr />
{% endif %}

{% assign talks_size = site.data.clunch | size %}
{% if talks_size > 0 %}
  <p>
  <h2>Past Talks</h2>

  {% for talk in site.data.clunch %}
    {% include talk.html speaker=talk.speaker url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
{% endif %}
