---
layout: page
title: Projects
permalink: /projects/
description: Selected research experiments and robotics implementations
nav: true
nav_order: 4
---

<link rel="stylesheet" href="{{ '/assets/css/projects-portfolio.css' | relative_url }}">

<div class="ts-portfolio">
  <header class="ts-intro">
    <span class="ts-eyebrow">Research &amp; engineering</span>
    <h2>Control theory, tested in the loop.</h2>
    <p>Selected experiments and implementations in safety-critical control, state estimation, and autonomous systems.</p>
  </header>

  <div class="ts-section-bar">
    <h2>Selected projects</h2>
    <span>Simulation &middot; Robotics &middot; Experiments</span>
  </div>

  {% assign research_projects = site.projects | where: 'category', 'research' %}
  {% assign robotics_projects = site.projects | where: 'category', 'robotics' %}
  {% assign portfolio_projects = research_projects | concat: robotics_projects | sort: 'importance' %}

  <div class="ts-project-grid">
    {% for project in portfolio_projects %}
    <a class="ts-project-card{% if project.featured %} ts-project-card--feature{% endif %}" href="{{ project.url | relative_url }}" aria-label="Read about {{ project.title | escape }}">
      <div class="ts-card-visual">
        {% if project.img %}
          <img src="{{ project.img | relative_url }}" alt="{{ project.title | escape }}" loading="lazy">
        {% else %}
          <div class="ts-graphic" aria-hidden="true">
            <div class="ts-gridlines"></div>
            <div class="ts-orbit"></div>
            <div class="ts-orbit ts-orbit--inner"></div>
            <div class="ts-graphic-center"><strong>PX4</strong><small>Gazebo simulation</small></div>
          </div>
        {% endif %}
        <div class="ts-visual-top">{{ project.visual_label | default: 'CONTROL SYSTEMS' }}</div>
        <div class="ts-visual-bottom">
          <span>{{ project.category | upcase }}</span>
          {% if project.video_count %}<span>{{ project.video_count }} VIDEO{% if project.video_count != 1 %}S{% endif %}</span>{% endif %}
        </div>
      </div>
      <div class="ts-card-copy">
        <span class="ts-card-type">{{ project.kind | default: project.category }}</span>
        <h3>{{ project.title }}</h3>
        <p>{{ project.summary | default: project.description }}</p>
        {% if project.tags %}
        <div class="ts-tags">
          {% for tag in project.tags %}<span class="ts-tag">{{ tag }}</span>{% endfor %}
        </div>
        {% endif %}
        <span class="ts-card-link">Explore project <span aria-hidden="true">↗</span></span>
      </div>
    </a>
    {% endfor %}
  </div>
  {% if portfolio_projects.size == 0 %}
  <p class="ts-empty-note">Projects will appear here as they are added.</p>
  {% endif %}
</div>
