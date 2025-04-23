---
title: "Projects"
mathjax: true
layout: page
categories: media
---

<style>
.project-card {
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 1.5em;
  margin-bottom: 2em;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
}
.project-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}
.project-image {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  margin-bottom: 1em;
}
.project-title {
  font-size: 1.4em;
  font-weight: bold;
  margin-bottom: 0.5em;
}
.project-links a {
  margin-right: 1em;
  text-decoration: none;
  color: #005f99;
}
.project-links a:hover {
  text-decoration: underline;
}
</style>

<div class="project-card">
  <div class="project-title">
    Bird Call Recognition using Deep Learning and Acoustic-Based Feature Selection
  </div>
  <p>
    Processed 16K+ bird audio recordings into Mel spectrograms and acoustic features (MFCCs, spectral, rhythmic). Evaluated classical ML models and CNN-based pipelines to classify bird species in noisy environments, achieving 89.8% accuracy with Logistic Regression and improving preprocessing speed by 6x.
  </p>
</div>

<div class="project-card">
  <div class="project-title">
    Wildfire Modeling and Tree Species Classification
  </div>
  <p>
    Predicted plant functional type (PFT) and genus/species distributions using machine learning models on TLS-derived tree lists. Integrated field-collected data and FastFuels API to enhance labeling. Achieved 95%+ accuracy in PFT and 85% in species prediction across California field plots.
  </p>
  <div class="project-links">
    <a href="https://github.com/Shwyu/Fire-Ready-Forests-Data-Challenge" target="_blank">View on GitHub</a>
  </div>
</div>

<div class="project-card">
  <div class="project-title">
    Movie Recommendation System with Graph Database
  </div>
  <p>
    Built a graph-based movie recommender in Neo4j using 50K+ rows from IMDb and MovieLens datasets. Developed hybrid models combining collaborative and content-based filtering. Reduced Cypher query time by 3x and visualized genre and rating trends via Tableau dashboards.
  </p>
  <div class="project-links">
    <a href="https://github.com/Valier-Juri/DSC202-movie-recommendation-database" target="_blank">View on GitHub</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/telerobot2elderly.jpg" alt="Telepresence robot project" class="project-image">
  <div class="project-title">
    Telepresence Robot for Homebound Older Adults
  </div>
  <p>
    This project designs a conversational telepresence robot to assist homebound individuals in accessing botanical gardens remotely. Built with ROS, a mobile base, and a camera-equipped rod, it supports voice-driven navigation and GPT-powered plant explanations. Published at DIS 2024.
  </p>
  <div class="project-links">
    <a href="https://dl.acm.org/doi/pdf/10.1145/3643834.3660710" target="_blank">View Paper</a>
  </div>
</div>

<div class="project-card">
  <img src="/assets/6.jpg.png" alt="Voronoi diagram with Diestel-Leader graph" class="project-image">
  <div class="project-title">
    Diestel-Leader Graphs in Voronoi Diagrams
  </div>
  <p>
    Investigated the embedding of Diestel-Leader graphs in Voronoi diagrams and explored their topological implications in metric geometry. Developed during the UW–Madison MXM Seminar, this work bridges graph theory with spatial partitioning concepts.
  </p>
  <div class="project-links">
    <a href="../assets/MXM_Diestel_Leader_Voronoi.pdf" target="_blank">Poster</a>
    <a href="../assets/MXM_Paper_Diestel_Leader.pdf" target="_blank">Paper</a>
  </div>
</div>

