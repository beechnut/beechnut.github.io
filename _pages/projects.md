---
layout: page
title: Projects
---

<p>
  If you are interested in supporting or being a part of any of these projects,
  <br />
  <a href="mailto:cloyd.matt@gmail.com">please get in touch!</a> I'd love to meet you.
</p>

<br />

<div class="projects">
  {% for project in site.data.projects %}
    <h2>{{ project.name }}</h2>
    <h3>{{ project.tagline }}</h3>
    <img src="https://img.shields.io/static/v1?label=status&message={{project.status}}&color={{project.color}}" />
    {{ project.description | markdownify }}
    <strong>looking for</strong>: {{ project.looking_for }}
    <br />
    {% if project.link %}
      <a href="{{ project.link }}" target="_blank">{{ project.name }} -></a>
    {% endif %}


    <br />
    <br />
    <br />

  {% endfor %}
</div>
