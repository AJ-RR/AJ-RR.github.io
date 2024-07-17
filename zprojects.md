---
layout: page
title: Projects
permalink: /projects/
---

I have worked on several projects that span the following domains:
1. <a href="#Malaria Parasite Detection in Thin Blood Smear Images">Computer Vision</a>
2. <a href="#Speech Dialect Classification">Machine Learning and Signal Processing</a>
3. <a href="#Cognitive Radar - A Literature Review">Electronics and Embedded Systems</a>
4. <a href="#Motor Control Brain Implants - Design Considerations">Humanities and Social Sciences</a>

{% for project in site.projects %}
  <div class="project">
      <h3 id="{{project.title}}">{{project.title}}</h3>
      {{ project.from }} - {{ project.to }}<br>
      {% if project.role %}
        <i>{{ project.role }}</i>
      {% endif %}
      <p>
          {{ project.content }}
      </p>
      <div id="links">
        {% if project.code %}
          <a target="_blank" rel="noopener noreferrer" href="{{project.code}}">Code</a>&nbsp;&nbsp;&nbsp;
        {% endif %}
        {% if project.report %}
          <a target="_blank" rel="noopener noreferrer" href="{{project.report}}">Report</a>&nbsp;&nbsp;&nbsp;
        {% endif %}
        {% if project.link %}
          <a target="_blank" rel="noopener noreferrer" href="{{project.link}}">Link</a>
        {% endif %}
      </div>
  </div>
{% endfor %}