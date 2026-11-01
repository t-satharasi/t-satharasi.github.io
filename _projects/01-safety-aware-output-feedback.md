---
layout: page
title: Experimentation on Safety-Aware Output Feedback
permalink: /projects/safety-aware-output-feedback/
description: PX4 quadrotor experimentation in Gazebo using acceleration-level control
category: research
importance: 1
featured: true
github_url: https://github.com/t-satharasi/Safe-Output-Feedback-Control-via-SDRE-and-Barrier-States
kind: Simulation experiment
visual_label: Safety-aware output feedback
video_count: 1
summary: Simulation-based testing of safety-aware output-feedback control on a PX4 quadrotor in Gazebo, using an acceleration-level control interface.
tags:
  - PX4
  - Gazebo
  - Output Feedback
  - Safety-Critical Control
  - SDRE
  - Barrier States
video:
  title: PX4 / Gazebo Simulation Demonstration
  embed_url: https://drive.google.com/file/d/1iy9XiC47Icx7ujt07oWPPF_mGY242wqb/preview
  watch_url: https://drive.google.com/file/d/1iy9XiC47Icx7ujt07oWPPF_mGY242wqb/view?usp=sharing
  description: Safety-aware output-feedback control using acceleration-level commands in a Gazebo PX4 quadrotor simulation.
---

<link rel="stylesheet" href="{{ '/assets/css/projects-portfolio.css' | relative_url }}">

<article class="ts-case-study">
  <a class="ts-back-link" href="{{ '/projects/' | relative_url }}">← All projects</a>

  <header>
    <span class="ts-eyebrow">Simulation experiment &middot; Safety-critical control</span>
    <h1 class="ts-title">Experimentation on Safety-Aware Output Feedback</h1>
    <p class="ts-deck">An experimental implementation of safety-aware output-feedback control for a PX4 quadrotor in Gazebo, with control commands issued at the acceleration level.</p>
    <div class="ts-project-actions" aria-label="Project resources">
      <a class="ts-action ts-action--primary" href="{{ page.github_url }}" target="_blank" rel="noopener noreferrer" aria-label="View source code on GitHub (opens in a new tab)">
        <svg aria-hidden="true" viewBox="0 0 24 24" width="17" height="17" fill="currentColor"><path d="M12 .8A11.2 11.2 0 0 0 8.46 22.63c.56.1.76-.24.76-.54v-2.02c-3.1.67-3.76-1.32-3.76-1.32-.5-1.27-1.22-1.61-1.22-1.61-1.01-.69.08-.68.08-.68 1.12.08 1.71 1.14 1.71 1.14 1 .1.77 1.63 3.21 1.07.1-.72.39-1.22.71-1.5-2.47-.28-5.06-1.24-5.06-5.53 0-1.22.43-2.22 1.15-3-.11-.28-.5-1.42.11-2.96 0 0 .94-.3 3.08 1.15a10.76 10.76 0 0 1 5.6 0c2.14-1.45 3.08-1.15 3.08-1.15.61 1.54.22 2.68.11 2.96.72.78 1.15 1.78 1.15 3.01 0 4.3-2.59 5.24-5.07 5.52.4.35.76 1.03.76 2.07v3.07c0 .3.2.65.77.54A11.2 11.2 0 0 0 12 .8Z"/></svg>
        View source code <span aria-hidden="true">↗</span>
      </a>
      <a class="ts-action ts-action--secondary" href="#experiment-video">Watch experiment ↓</a>
    </div>
  </header>

  <div class="ts-specs" aria-label="Experiment specifications">
    <div class="ts-spec"><span class="ts-spec-label">Flight platform</span><span class="ts-spec-value">PX4 quadrotor</span></div>
    <div class="ts-spec"><span class="ts-spec-label">Simulation</span><span class="ts-spec-value">Gazebo</span></div>
    <div class="ts-spec"><span class="ts-spec-label">Control interface</span><span class="ts-spec-value">Acceleration level</span></div>
  </div>

  <section id="experiment-video" aria-labelledby="ts-recordings-heading">
    <div class="ts-content-heading"><h2 id="ts-recordings-heading">Experiment video</h2><span>Simulation demonstration</span></div>
    <div class="ts-videos">
      <div class="ts-video-card">
        <div class="ts-video-frame">
          <iframe
            src="{{ page.video.embed_url }}"
            title="{{ page.video.title | escape }}"
            loading="lazy"
            allow="autoplay; fullscreen; picture-in-picture"
            allowfullscreen>
          </iframe>
        </div>
        <div class="ts-video-meta">
          <h3>{{ page.video.title }}</h3>
          <p>{{ page.video.description }}</p>
          <a class="ts-video-external" href="{{ page.video.watch_url }}" target="_blank" rel="noopener noreferrer">Watch on Google Drive ↗</a>
        </div>
      </div>
    </div>
  </section>

  <section class="ts-about-grid" aria-label="Experiment details">
    <div>
      <h2>Overview</h2>
      <p>This project examines safety-aware output-feedback control in a simulated quadrotor environment. The implementation uses PX4 with Gazebo, and the controller operates through acceleration-level commands. The experiment is presented in a single demonstration video.</p>
    </div>
    <div>
      <h2>Experimental setup</h2>
      <ul>
        <li><strong>Vehicle:</strong> PX4 quadrotor</li>
        <li><strong>Environment:</strong> Gazebo simulation</li>
        <li><strong>Control:</strong> Acceleration-level interface</li>
        <li><strong>Media:</strong> One experiment video</li>
      </ul>
    </div>
  </section>

  <p class="ts-note">The specific test objectives and observations can be added alongside the video once the footage is available. No performance or safety claims are made without an accompanying evaluation.</p>
</article>
