---
layout: page
title: Safety-Aware Output-Feedback Control
permalink: /projects/safety-aware-output-feedback/
description: PX4 quadrotor simulation in Gazebo with acceleration-level control
category: research
importance: 1
---

<style>
  .ts-project-detail { max-width: 850px; }
  .ts-project-detail .eyebrow { color: var(--global-theme-color, #127c85); text-transform: uppercase; font-size: .78rem; font-weight: 700; letter-spacing: .08em; }
  .ts-project-detail .lead { font-size: 1.1rem; line-height: 1.7; margin: .8rem 0 1.5rem; }
  .ts-project-detail .actions { display: flex; flex-wrap: wrap; gap: .7rem; margin-bottom: 1.5rem; }
  .ts-project-detail .actions a { display: inline-block; border: 1px solid var(--global-theme-color, #127c85); color: var(--global-theme-color, #127c85); border-radius: 8px; padding: .55rem .95rem; text-decoration: none; font-weight: 600; }
  .ts-project-detail .facts { display: flex; flex-wrap: wrap; gap: .7rem; margin-bottom: 2rem; }
  .ts-project-detail .facts span { border: 1px solid var(--global-divider-color, #d5dce2); border-radius: 8px; padding: .65rem .9rem; font-size: .9rem; }
  .ts-project-detail .video { position: relative; width: 100%; padding-top: 56.25%; border-radius: 12px; overflow: hidden; background: #102734; }
  .ts-project-detail .video iframe { position: absolute; inset: 0; width: 100%; height: 100%; border: 0; }
  .ts-project-detail .external { margin: .7rem 0 2rem; font-size: .9rem; }
</style>

<article class="ts-project-detail">
  <p class="eyebrow">Safety-critical control · Simulation</p>
  <p class="lead">A simulation demonstration of safety-aware output-feedback control on a PX4 quadrotor in Gazebo, using acceleration-level commands.</p>

  <div class="actions">
    <a href="https://github.com/t-satharasi/Safe-Output-Feedback-Control-via-SDRE-and-Barrier-States" target="_blank" rel="noopener noreferrer">GitHub source code ↗</a>
    <a href="#demonstration">Watch experiment ↓</a>
  </div>

  <div class="facts">
    <span><strong>Platform:</strong> PX4 quadrotor</span>
    <span><strong>Environment:</strong> Gazebo</span>
    <span><strong>Control:</strong> Acceleration level</span>
  </div>

  <h2 id="demonstration">Experiment video</h2>
  <div class="video">
    <iframe src="https://drive.google.com/file/d/1iy9XiC47Icx7ujt07oWPPF_mGY242wqb/preview" title="Safety-aware output-feedback PX4 Gazebo simulation" loading="lazy" allow="autoplay; fullscreen" allowfullscreen></iframe>
  </div>
  <p class="external"><a href="https://drive.google.com/file/d/1iy9XiC47Icx7ujt07oWPPF_mGY242wqb/view?usp=sharing" target="_blank" rel="noopener noreferrer">Open video in Google Drive ↗</a></p>

  <h2>Overview</h2>
  <p>This project investigates safety-aware output-feedback control in a simulated quadrotor environment. The implementation uses a PX4 flight stack with a Gazebo simulator and an acceleration-level control interface.</p>
</article>
