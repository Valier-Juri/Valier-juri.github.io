---
title: "Projects"
mathjax: true
layout: page
categories: media
permalink: /project
---

<style>
.project-row {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 2em;
  margin-bottom: 3em;
  padding: 1em;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
  background-color: #fafafa;
}

.project-row:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
}

/* Dark Mode Support for Projects */
@media (prefers-color-scheme: dark) {
  .project-row {
    background-color: #1a1a1a !important;
    border-color: rgba(74, 144, 226, 0.4) !important;
    box-shadow: 0 2px 6px rgba(0,0,0,0.3) !important;
    color: #ffffff !important;
  }

  .project-row:hover {
    background-color: #2d2d2d !important;
    box-shadow: 0 4px 12px rgba(0,0,0,0.5) !important;
  }

  .project-title {
    color: #ffffff !important;
  }

  .project-content {
    color: #ffffff !important;
  }

  .project-content p {
    color: #e0e0e0 !important;
  }
}

/* Force Dark Mode for Projects */
[data-theme="dark"] .project-row,
.dark-mode .project-row,
html[data-bs-theme="dark"] .project-row {
  background-color: #1a1a1a !important;
  border-color: rgba(74, 144, 226, 0.4) !important;
  box-shadow: 0 2px 6px rgba(0,0,0,0.3) !important;
  color: #ffffff !important;
}

[data-theme="dark"] .project-row:hover,
.dark-mode .project-row:hover,
html[data-bs-theme="dark"] .project-row:hover {
  background-color: #2d2d2d !important;
  box-shadow: 0 4px 12px rgba(0,0,0,0.5) !important;
}

[data-theme="dark"] .project-title,
.dark-mode .project-title,
html[data-bs-theme="dark"] .project-title {
  color: #ffffff !important;
}

[data-theme="dark"] .project-content,
.dark-mode .project-content,
html[data-bs-theme="dark"] .project-content {
  color: #ffffff !important;
}

[data-theme="dark"] .project-content p,
.dark-mode .project-content p,
html[data-bs-theme="dark"] .project-content p {
  color: #e0e0e0 !important;
}

.project-image {
  flex: 0 0 200px;
  max-width: 200px;
  border-radius: 8px;
  object-fit: cover;
}

.project-content {
  flex: 1;
}

.project-title {
  font-size: 1.3em;
  font-weight: bold;
  margin-bottom: 0.4em;
}

.project-links {
  margin-top: 0.8em;
}

.project-links a {
  font-size: 0.95em;
  margin-right: 1em;
  text-decoration: none;
  color: #007acc;
}

.project-links a:hover {
  text-decoration: underline;
}

/* Dark Mode Support for Project Links */
@media (prefers-color-scheme: dark) {
  .project-links a {
    color: #4A90E2 !important;
  }

  .project-links a:hover {
    color: #6BB6FF !important;
  }
}

/* Force Dark Mode for Project Links */
[data-theme="dark"] .project-links a,
.dark-mode .project-links a,
html[data-bs-theme="dark"] .project-links a {
  color: #4A90E2 !important;
}

[data-theme="dark"] .project-links a:hover,
.dark-mode .project-links a:hover,
html[data-bs-theme="dark"] .project-links a:hover {
  color: #6BB6FF !important;
}

/* Mobile Responsive Design for Projects */
@media (max-width: 768px) {
  .project-row {
    flex-direction: column;
    gap: 1em;
    padding: 0.8em;
    margin-bottom: 2em;
  }

  .project-image {
    flex: none;
    max-width: 100%;
    width: 100%;
    height: auto;
    max-height: 200px;
  }

  .project-title {
    font-size: 1.2em;
  }

  .project-content p {
    font-size: 0.9em;
    line-height: 1.5;
  }

  .project-links {
    margin-top: 0.6em;
  }

  .project-links a {
    display: inline-block;
    margin-bottom: 0.5em;
    padding: 0.5em 1em;
    background: rgba(0, 122, 204, 0.1);
    border-radius: 5px;
    border: 1px solid rgba(0, 122, 204, 0.3);
  }
}

@media (max-width: 480px) {
  .project-row {
    padding: 0.6em;
    margin-bottom: 1.5em;
  }

  .project-title {
    font-size: 1.1em;
  }

  .project-content p {
    font-size: 0.85em;
  }

  .project-links a {
    font-size: 0.9em;
    padding: 0.4em 0.8em;
  }
}
</style>

<div class="project-row">
  <img src="/assets/bird-preview.png" alt="Bird project" class="project-image">
  <div class="project-content">
    <div class="project-title">Bird Call Recognition - Bird CLEF</div>
    <p>A sound-based classification project focused on identifying bird species from field recordings. The pipeline involves converting raw audio into spectrograms and engineered acoustic features, and training both classical and deep learning models for species recognition.</p>
  </div>
</div>

<div class="project-row">
  <img src="/assets/fire-preview.jpg.png" alt="Tree Species Classification" class="project-image">
  <div class="project-content">
    <div class="project-title">ML Modeling and Tree Species Classification</div>
    <p>This project explores how forest plot data can be used to infer ecological characteristics at scale. Using 3D laser scan inputs and government tree inventories, it predicts the distribution of vegetation types and species in wildfire-prone regions of California.</p>
    <div class="project-links">
      <a href="https://github.com/Shwyu/Fire-Ready-Forests-Data-Challenge" target="_blank">View on GitHub</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/movie-preview.jpg.png" alt="Movie Recommendation" class="project-image">
  <div class="project-content">
    <div class="project-title">Movie Recommendation System with Graph Database</div>
    <p>A recommender engine built on graph structures, combining user behavior and movie metadata. The system uses Neo4j to represent relationships between viewers, genres, and ratings, and delivers hybrid suggestions through both collaborative and content-based strategies.</p>
    <div class="project-links">
      <a href="https://github.com/Valier-Juri/DSC202-movie-recommendation-database" target="_blank">View on GitHub</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/telerobot2elderly.jpg" alt="Telepresence robot project" class="project-image">
  <div class="project-content">
    <div class="project-title">Telepresence Robot for Homebound Older Adults</div>
    <p>This project designs a conversational telepresence robot to assist homebound individuals in accessing botanical gardens remotely. Built with ROS, a mobile base, and a camera-equipped rod, it supports voice-driven navigation and GPT-powered plant explanations. Published at DIS 2024.</p>
    <div class="project-links">
      <a href="https://dl.acm.org/doi/pdf/10.1145/3643834.3660710" target="_blank">View Paper</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/6.jpg.png" alt="Voronoi diagram with Diestel-Leader graph" class="project-image">
  <div class="project-content">
    <div class="project-title">Diestel-Leader Graphs in Voronoi Diagrams</div>
    <p>Investigated the embedding of Diestel-Leader graphs in Voronoi diagrams and explored their topological implications in metric geometry. Developed during the UW–Madison MXM Seminar, this work bridges graph theory with spatial partitioning concepts.</p>
    <div class="project-links">
      <a href="/assets/MXM_Diestel_Leader_Voronoi.pdf" target="_blank">Poster</a>
      <a href="/assets/MXM_Paper_Diestel_Leader.pdf" target="_blank">Paper</a>
    </div>
  </div>
</div>
