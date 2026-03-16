---
layout: archive
title: "Tools"
permalink: /tools/
author_profile: true
redirect_from: 
  - /tools.html
---

<style>
  .tools-intro {
    font-size: 1.05rem;
    color: #555;
    margin-bottom: 2.5rem;
    line-height: 1.7;
  }

  .tools-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 1.8rem;
    margin-top: 1rem;
  }

  .tool-card {
    background: #ffffff;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 1.6rem 1.8rem;
    text-decoration: none !important;
    color: inherit !important;
    display: block;
    transition: all 0.25s ease;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    position: relative;
    overflow: hidden;
  }

  .tool-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: linear-gradient(90deg, #1a5276, #2980b9, #1abc9c);
    opacity: 0;
    transition: opacity 0.25s ease;
  }

  .tool-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
    border-color: #b0c4de;
    text-decoration: none !important;
  }

  .tool-card:hover::before {
    opacity: 1;
  }

  .tool-card .card-icon {
    font-size: 2rem;
    margin-bottom: 0.8rem;
  }

  .tool-card .card-title {
    font-size: 1.1rem;
    font-weight: 700;
    color: #1a3a5c;
    margin-bottom: 0.5rem;
    letter-spacing: -0.01em;
  }

  .tool-card .card-desc {
    font-size: 0.88rem;
    color: #666;
    line-height: 1.6;
    margin-bottom: 1rem;
  }

  .tool-card .card-tag {
    display: inline-block;
    background: #eaf2fb;
    color: #1a5276;
    font-size: 0.75rem;
    font-weight: 600;
    padding: 2px 10px;
    border-radius: 20px;
    letter-spacing: 0.03em;
  }

  .card-arrow {
    position: absolute;
    bottom: 1.2rem;
    right: 1.5rem;
    color: #aaa;
    font-size: 1.1rem;
    transition: transform 0.2s, color 0.2s;
  }

  .tool-card:hover .card-arrow {
    transform: translateX(4px);
    color: #2980b9;
  }

  .section-label {
    font-size: 0.75rem;
    font-weight: 700;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: #999;
    margin-bottom: 1.2rem;
    padding-bottom: 0.4rem;
    border-bottom: 1px solid #eee;
  }

  /* Coming soon card style */
  .tool-card.coming-soon {
    opacity: 0.6;
    cursor: default;
    pointer-events: none;
  }

  .tool-card.coming-soon .card-tag {
    background: #f0f0f0;
    color: #999;
  }
</style>

<p class="tools-intro">
  A growing collection of interactive tools and utilities for astrophysics and cosmology research.
  Each tool is designed to be fast, precise, and reference-quality.
</p>

<div class="section-label">🔭 Cosmology &amp; Astrophysics</div>

<div class="tools-grid">

  <a class="tool-card" href="/tools/cosmology-calculator.html">
    <div class="card-icon">🌌</div>
    <div class="card-title">Cosmology Calculator</div>
    <div class="card-desc">
      Compute cosmological distances, times and universe contents
      from given redshift <em>z</em>
    </div>
    <span class="card-tag">Interactive Tool</span>
    <span class="card-arrow">→</span>
  </a>

  <div class="tool-card coming-soon">
    <div class="card-icon">⭐</div>
    <div class="card-title">Stellar Evolution Tracks</div>
    <div class="card-desc">
      Visualize stellar evolutionary tracks on the HR diagram for different masses and metallicities.
    </div>
    <span class="card-tag">Coming Soon</span>
  </div>

  <div class="tool-card coming-soon">
    <div class="card-icon">🌀</div>
    <div class="card-title">Halo Mass Function</div>
    <div class="card-desc">
      Compute dark matter halo mass functions using Press-Schechter and calibrated fitting formulae.
    </div>
    <span class="card-tag">Coming Soon</span>
  </div>

</div>
