---
layout: page
title: Projects
permalink: /projects/
---

<ul class="listing">
{% for project in site.projects %}
  <li class="listing-item">
    <h2>{{ project.title }}</h2>
    <div class="post-meta">
    {{project.description}}
    </div>
    <br/>
    <img src="images/{{project.image}}" height="400px" allign="left" style="margin-top: 0px"/>
    <p>{{project.content}}</p>
    <div class="post-meta">
    {% if project.video %}
    <a href="{{project.video}}" rel="noopener noreferrer" target="_blank">Video Demo</a>
    <br/>
    {% endif %}
    {% if project.download %}
    <a href="{{project.download}}" rel="noopener noreferrer" target="_blank">Download</a>
    <br/>
    {% endif %}
    {% if project.link %}
    <a href="{{project.link}}" rel="noopener noreferrer" target="_blank">Live Web App Demo</a>
    <br/>
    {% endif %}
    {% if project.github %}
    <a href="{{project.github}}" rel="noopener noreferrer" target="_blank">Github</a>
    {% endif %}
    </div>
  </li>
{% endfor %}
</ul>