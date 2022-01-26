---
layout: default
title: CLunch
order: 3
---
# CLunch
CLunch is the weekly <b>C</b>omputational <b>L</b>inguistics l<b>unch</b> run by the NLP group.
We invite external and internal speakers to come and present their research on natural language processing, computational linguistics, and machine learning.

Interested in attending CLunch? Sign up for our mailing list [here](http://lists.seas.upenn.edu/mailman/listinfo/clunch).

View older talks at the [CLunch archive](/clunch_archive).

{% assign future_talks_size = site.data.future_clunch | size %}
{% if future_talks_size > 0 %}
  <p>
  <h2>Upcoming Talks</h2>
  <h3>Spring 2022</h3>

  {% for talk in site.data.future_clunch %}
    {% include talk.html speaker=talk.speaker img=talk.img url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
{% endif %}

{% assign talks_size = site.data.clunch | size %}
{% if talks_size > 0 %}
  <p>
  <h2>Past Talks</h2>
  <h3>Fall 2021</h3>
  <p markdown="1">
  Past talks from the current and previous semesters are shown below. View older talks at the [CLunch archive](/clunch_archive).
  </p>
  {% for talk in site.data.clunch %}
    {% include talk.html speaker=talk.speaker img=talk.img url=talk.url title=talk.title abstract=talk.abstract date=talk.date affiliation=talk.affiliation %}
  {% endfor %}
  </p>
{% endif %}
