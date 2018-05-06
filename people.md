---
layout: default
title: People
---
<style type="text/css">
  .people {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
  }
</style>

<h1>People</h1>

<h2>Faculty</h2>
<p>
  <div class="people">
    {% for person in site.data.people %}
      {% if person.status == "faculty" %}
        {% include person.html name=person.name img=person.img url=person.url %}
      {% endif %}
    {% endfor %}
  </div>
</p>

<h2>Ph.D. Students</h2>
<p>
  <div class="people">
    {% for person in site.data.people %}
      {% if person.status == "phd" %}
        {% include person.html name=person.name img=person.img url=person.url %}
      {% endif %}
    {% endfor %}
  </div>
</p>

<h2>Master's Students</h2>
<p>
  <div class="people">
    {% for person in site.data.people %}
      {% if person.status == "masters" %}
        {% include person.html name=person.name img=person.img url=person.url %}
      {% endif %}
    {% endfor %}
  </div>
</p>

<h2>Undergraduates</h2>
<p>
  <div class="people">
    {% for person in site.data.people %}
      {% if person.status == "undergrad" %}
        {% include person.html name=person.name img=person.img url=person.url %}
      {% endif %}
    {% endfor %}
  </div>
</p>

<h2>Alumni</h2>
Check out our many, many alumni <a href="/alumni">here</a>.
