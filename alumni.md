---
layout: default
title: Alumni
order: 2
---
<h1>Alumni</h1>
Missing from this list? New position? Contact <a href="http://veronica320.github.io">Veronica Qing Lyu</a> for help.

<h2>2020's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 2020 <= person.year and person.year <= 2029  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>

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

<h2>1980's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 1980 <= person.year and person.year <= 1989  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>

<h2>1970's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 1970 <= person.year and person.year <= 1979  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>

<h2>1960's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 1960 <= person.year and person.year <= 1969  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>

<h2>1950's</h2>
<p>
  {% for person in site.data.alumni %}
    {% if 1950 <= person.year and person.year <= 1959  %}
      {% include alumnus.html name=person.name url=person.url year=person.year degree=person.degree current=person.current %}
    {% endif %}
  {% endfor %}
</p>
