---
layout: page
title: Projects
permalink: /projects/
---

I have worked on several projects that span the following domains:
1. <a href="#Microsurgical Tool Detection and Characterization in Intra-operative Neurosurgical Videos">Computer Vision</a>
2. <a href="#Cognitive Radar: A Literature Review">Machine Learning and Signal Processing</a>
4. <a href = "#Modeling Influencer Marketing Campaigns In Social Networks">Computer Programming</a>
3. <a href="#Tactile Educational Kit for Students with Visual Impairment">Electronics and Embedded Systems</a>
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