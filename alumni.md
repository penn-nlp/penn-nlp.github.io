---
layout: default
title: Alumni
---
<h1>Alumni</h1>
Missing from this list? New position? Contact <a href="http://danieldeutsch.github.io">Dan Deutsch</a> for help.

<h2>2010's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 2010 <= person.year and person.year <= 2019  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>
