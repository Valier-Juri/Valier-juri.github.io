---
title: "Projects"
mathjax: true
layout: page
categories: media
permalink: /project
---

<div class="page-intro">
  <p>我的研究和项目集中在机器学习、计算机视觉和人机交互领域。这些项目展示了我对技术如何解决现实世界问题的探索，特别是在生态、自然和人类中心的应用方面。</p>
</div>

<style>
.page-intro {
  margin-bottom: 2.5em;
  padding-bottom: 1.5em;
  border-bottom: 1px solid rgba(169, 132, 103, 0.2);
}

.project-row {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 2.5em;
  margin-bottom: 3.5em;
  padding: 1.5em;
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.06);
  background-color: #fff;
  transition: transform 0.4s ease, box-shadow 0.4s ease;
}

.project-row:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 25px rgba(0,0,0,0.1);
}

.project-image {
  flex: 0 0 280px;
  max-width: 280px;
  height: 200px;
  border-radius: 8px;
  object-fit: cover;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  transition: transform 0.5s ease;
}

.project-row:hover .project-image {
  transform: scale(1.03);
}

.project-content {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.project-title {
  font-family: "Playfair Display", Georgia, serif;
  font-size: 1.5em;
  font-weight: 600;
  margin-bottom: 0.6em;
  color: #4A4A4A;
}

.project-description {
  line-height: 1.7;
  margin-bottom: 1.2em;
  color: #555;
  flex-grow: 1;
}

.project-links {
  margin-top: 0.8em;
}

.project-links a {
  font-size: 0.95em;
  margin-right: 1.5em;
  text-decoration: none;
  color: #A98467;
  padding: 0.3em 0;
  position: relative;
  font-weight: 500;
  transition: color 0.3s ease;
}

.project-links a::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0;
  height: 2px;
  background-color: #A98467;
  transition: width 0.3s ease;
}

.project-links a:hover {
  color: #7D8C85;
  text-decoration: none;
}

.project-links a:hover::after {
  width: 100%;
}

.project-tag {
  display: inline-block;
  background-color: rgba(169, 132, 103, 0.1);
  color: #7D8C85;
  padding: 0.2em 0.8em;
  border-radius: 20px;
  font-size: 0.85em;
  margin-right: 0.5em;
  margin-bottom: 0.5em;
}

@media (max-width: 768px) {
  .project-row {
    flex-direction: column;
    padding: 1em;
  }
  
  .project-image {
    flex: 0 0 auto;
    max-width: 100%;
    margin-bottom: 1.2em;
  }
}
</style>

<div class="project-row">
  <img src="/assets/bird-preview.png" alt="Bird project" class="project-image">
  <div class="project-content">
    <div class="project-title">Bird Call Recognition - Bird CLEF</div>
    <p class="project-description">A sound-based classification project focused on identifying bird species from field recordings. The pipeline involves converting raw audio into spectrograms and engineered acoustic features, and training both classical and deep learning models for species recognition.</p>
    <div class="project-tags">
      <span class="project-tag">音频处理</span>
      <span class="project-tag">深度学习</span>
      <span class="project-tag">生态保护</span>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/fire-preview.jpg.png" alt="Tree Species Classification" class="project-image">
  <div class="project-content">
    <div class="project-title">ML Modeling and Tree Species Classification</div>
    <p class="project-description">This project explores how forest plot data can be used to infer ecological characteristics at scale. Using 3D laser scan inputs and government tree inventories, it predicts the distribution of vegetation types and species in wildfire-prone regions of California.</p>
    <div class="project-tags">
      <span class="project-tag">机器学习</span>
      <span class="project-tag">3D数据</span>
      <span class="project-tag">环境科学</span>
    </div>
    <div class="project-links">
      <a href="https://github.com/Shwyu/Fire-Ready-Forests-Data-Challenge" target="_blank">查看源代码</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/movie-preview.jpg.png" alt="Movie Recommendation" class="project-image">
  <div class="project-content">
    <div class="project-title">Movie Recommendation System with Graph Database</div>
    <p class="project-description">A recommender engine built on graph structures, combining user behavior and movie metadata. The system uses Neo4j to represent relationships between viewers, genres, and ratings, and delivers hybrid suggestions through both collaborative and content-based strategies.</p>
    <div class="project-tags">
      <span class="project-tag">图数据库</span>
      <span class="project-tag">Neo4j</span>
      <span class="project-tag">推荐系统</span>
    </div>
    <div class="project-links">
      <a href="https://github.com/Valier-Juri/DSC202-movie-recommendation-database" target="_blank">查看源代码</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/telerobot2elderly.jpg" alt="Telepresence robot project" class="project-image">
  <div class="project-content">
    <div class="project-title">Telepresence Robot for Homebound Older Adults</div>
    <p class="project-description">This project designs a conversational telepresence robot to assist homebound individuals in accessing botanical gardens remotely. Built with ROS, a mobile base, and a camera-equipped rod, it supports voice-driven navigation and GPT-powered plant explanations. Published at DIS 2024.</p>
    <div class="project-tags">
      <span class="project-tag">机器人</span>
      <span class="project-tag">人机交互</span>
      <span class="project-tag">ROS</span>
      <span class="project-tag">已发表论文</span>
    </div>
    <div class="project-links">
      <a href="https://dl.acm.org/doi/pdf/10.1145/3643834.3660710" target="_blank">阅读论文</a>
    </div>
  </div>
</div>

<div class="project-row">
  <img src="/assets/6.jpg.png" alt="Voronoi diagram with Diestel-Leader graph" class="project-image">
  <div class="project-content">
    <div class="project-title">Diestel-Leader Graphs in Voronoi Diagrams</div>
    <p class="project-description">Investigated the embedding of Diestel-Leader graphs in Voronoi diagrams and explored their topological implications in metric geometry. Developed during the UW–Madison MXM Seminar, this work bridges graph theory with spatial partitioning concepts.</p>
    <div class="project-tags">
      <span class="project-tag">图论</span>
      <span class="project-tag">几何</span>
      <span class="project-tag">数学研究</span>
    </div>
    <div class="project-links">
      <a href="/assets/MXM_Diestel_Leader_Voronoi.pdf" target="_blank">查看海报</a>
      <a href="/assets/MXM_Paper_Diestel_Leader.pdf" target="_blank">阅读论文</a>
    </div>
  </div>
</div>
