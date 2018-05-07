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

<h2>2000's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 2000 <= person.year and person.year <= 2009  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>

<h2>1990's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 1990 <= person.year and person.year <= 1999  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>
