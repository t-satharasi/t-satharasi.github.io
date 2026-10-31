---
layout: page
title: Experimentation on Safety-Aware Output Feedback
permalink: /projects/safety-aware-output-feedback/
description: PX4 quadrotor experimentation in Gazebo using acceleration-level control
category: research
importance: 1
featured: true
kind: Simulation experiment
visual_label: Safety-aware output feedback
video_count: 1
summary: Simulation-based testing of safety-aware output-feedback control on a PX4 quadrotor in Gazebo, using an acceleration-level control interface.
tags:
  - PX4
  - Gazebo
  - Output Feedback
  - Safety-Critical Control
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
  </header>

  <div class="ts-specs" aria-label="Experiment specifications">
    <div class="ts-spec"><span class="ts-spec-label">Flight platform</span><span class="ts-spec-value">PX4 quadrotor</span></div>
    <div class="ts-spec"><span class="ts-spec-label">Simulation</span><span class="ts-spec-value">Gazebo</span></div>
    <div class="ts-spec"><span class="ts-spec-label">Control interface</span><span class="ts-spec-value">Acceleration level</span></div>
  </div>

  <section aria-labelledby="ts-recordings-heading">
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
