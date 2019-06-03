---
layout: page
title: Projects
permalink: /projects/
---

<ul class="listing">
{% for project in site.projects %}
  <li class="listing-item">
    <h2>{{ project.title }} - {{project.purpose}}</h2>
    <div class="post-meta">
    {{project.description}}
    </div>
    <br/>
    <img src="images/{{project.image}}" height="300px" allign="left" style="margin-top: 0px"/>
    <p>{{project.content}}</p>
    <div class="post-meta">
    {% if project.github %}
    <a href="{{project.github}}" rel="noopener noreferrer" target="_blank">Github</a>
    {% endif %}
    {% if project.download %}
    <br/>
    <a href="{{project.download}}" rel="noopener noreferrer" target="_blank">Download</a>
    {% endif %}
    </div>
  </li>
{% endfor %}
</ul>