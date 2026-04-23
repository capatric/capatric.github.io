---
layout: default
title: Home
description: Carlos Patricio builds reliable AI infrastructure and Linux automation for cloud and hardware-heavy environments.
---

<section class="hero">
  <p class="eyebrow">Oracle | Site Reliability Engineering</p>
  <h1>Reliable infrastructure for AI systems, Linux platforms, and hardware-heavy operations.</h1>
  <p class="lead">I’m Carlos Patricio, an Electronics Engineer and Site Reliability Engineer working at the intersection of cloud infrastructure, system validation, and automation. I focus on keeping demanding environments observable, reproducible, and stable under pressure.</p>
  <div class="hero-actions">
    <a class="button button-primary" href="{{ '/about' | relative_url }}">View experience</a>
    <a class="button button-secondary" href="{{ '/posts' | relative_url }}">Read notes</a>
  </div>
</section>

<section class="section-block">
  <div class="section-heading">
    <h2>What I work on</h2>
    <p>My background spans cloud operations and low-level validation work, which makes me comfortable moving between software reliability and hardware-aware debugging.</p>
  </div>

  <div class="feature-grid">
    <article class="feature-card">
      <h3>AI infrastructure reliability</h3>
      <p>Production-minded operations for systems that need strong observability, predictable recovery paths, and disciplined change management.</p>
    </article>
    <article class="feature-card">
      <h3>Linux and automation</h3>
      <p>Operational tooling in Python and Bash to reduce manual work, standardize workflows, and surface failures early.</p>
    </article>
    <article class="feature-card">
      <h3>Hardware validation</h3>
      <p>Experience in bring-up, electrical validation, and lab automation for complex platforms where software and hardware constraints meet.</p>
    </article>
  </div>
</section>

<section class="section-block">
  <div class="section-heading">
    <h2>Recent writing</h2>
    <p>Short notes on reliability, validation, and the operational habits that make technical systems easier to trust.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts limit:3 %}
    <article class="post-card">
      <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <a class="text-link" href="{{ post.url }}">Read post</a>
    </article>
    {% endfor %}
  </div>
</section>
