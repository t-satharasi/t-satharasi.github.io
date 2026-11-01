---
layout: page
title: Projects
permalink: /projects/
description: Research and experimental implementations
nav: true
nav_order: 4
---

<style>
  .ts-project-intro { margin: 0 0 2rem; }
  .ts-project-intro p { color: var(--global-text-color); opacity: .8; max-width: 660px; }
  .ts-project-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 340px), 1fr)); gap: 1.25rem; }
  .ts-project-card { display: block; padding: 1.5rem; border: 1px solid var(--global-divider-color, #d5dce2); border-radius: 14px; text-decoration: none !important; color: inherit !important; transition: border-color .2s, transform .2s; }
  .ts-project-card:hover { border-color: var(--global-theme-color, #127c85); transform: translateY(-2px); }
  .ts-project-card .tag { color: var(--global-theme-color, #127c85); font-size: .75rem; letter-spacing: .08em; text-transform: uppercase; font-weight: 700; }
  .ts-project-card h3 { margin: .7rem 0; font-size: 1.2rem; }
  .ts-project-card p { margin: 0 0 1.2rem; opacity: .78; }
  .ts-project-card .cta { color: var(--global-theme-color, #127c85); font-weight: 600; }
</style>

<section class="ts-project-intro">
  <h2>Research &amp; engineering</h2>
  <p>Selected implementations in safety-critical control, estimation, and autonomous systems.</p>
</section>

<div class="ts-project-grid">
  {% assign ordered_projects = site.projects | sort: 'importance' %}
  {% for project in ordered_projects %}
    {% if project.category == 'research' or project.category == 'robotics' %}
      <a class="ts-project-card" href="{{ project.url | relative_url }}">
        <span class="tag">{{ project.category }}</span>
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <span class="cta">View project ↗</span>
      </a>
    {% endif %}
  {% endfor %}
</div>
