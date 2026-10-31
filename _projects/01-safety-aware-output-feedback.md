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
video_count: 3
summary: Simulation-based testing of safety-aware output-feedback control on a PX4 quadrotor in Gazebo, using an acceleration-level control interface.
tags:
  - PX4
  - Gazebo
  - Output Feedback
  - Safety-Critical Control
videos:
  - title: Recording 01
    src: /assets/video/safety-aware-output-feedback/recording-01.mp4
    description: First recorded simulation run.
    ready: false
  - title: Recording 02
    src: /assets/video/safety-aware-output-feedback/recording-02.mp4
    description: Second recorded simulation run.
    ready: false
  - title: Recording 03
    src: /assets/video/safety-aware-output-feedback/recording-03.mp4
    description: Third recorded simulation run.
    ready: false
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
    <div class="ts-content-heading"><h2 id="ts-recordings-heading">Experiment recordings</h2><span>Three simulation videos</span></div>
    <div class="ts-videos">
      {% for video in page.videos %}
      <div class="ts-video-card">
        <div class="ts-video-frame">
          {% if video.ready %}
          <video controls playsinline preload="metadata" aria-label="{{ video.title | escape }}">
            <source src="{{ video.src | relative_url }}" type="video/mp4">
            Your browser does not support HTML5 video.
          </video>
          {% else %}
          <div class="ts-video-no">Experiment {{ forloop.index | prepend: '0' }}</div>
          <div class="ts-video-pending"><strong>Video slot {{ forloop.index }}</strong><span>Recording to be uploaded</span></div>
          {% endif %}
        </div>
        <div class="ts-video-meta"><h3>{{ video.title }}</h3><p>{{ video.description }}</p></div>
      </div>
      {% endfor %}
    </div>
  </section>

  <section class="ts-about-grid" aria-label="Experiment details">
    <div>
      <h2>Overview</h2>
      <p>This project examines safety-aware output-feedback control in a simulated quadrotor environment. The implementation uses PX4 with Gazebo, and the controller operates through acceleration-level commands. Three recorded simulation runs document the experiments.</p>
    </div>
    <div>
      <h2>Experimental setup</h2>
      <ul>
        <li><strong>Vehicle:</strong> PX4 quadrotor</li>
        <li><strong>Environment:</strong> Gazebo simulation</li>
        <li><strong>Control:</strong> Acceleration-level interface</li>
        <li><strong>Media:</strong> Three recorded runs</li>
      </ul>
    </div>
  </section>

  <p class="ts-note">The individual test objectives and observations will be added alongside the recordings. No performance or safety claims are made from the videos without an accompanying evaluation.</p>
</article>
