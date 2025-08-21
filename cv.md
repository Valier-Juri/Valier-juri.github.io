---
title:  "Resume"
mathjax: true
layout: post
categories: media
---

<div class="resume-container">
  <object data="/assets/Resume_manlinzhang.pdf" width="100%" height="100%" type='application/pdf'></object>
</div>

<!-- 添加移动端备用链接 -->
<div class="mobile-pdf-link">
  <p>如果PDF无法正常显示，请<a href="/assets/Resume_manlinzhang.pdf" target="_blank">点击这里</a>直接查看或下载。</p>
</div>

<style>
  .resume-container {
    width: 100%;
    max-width: 800px;
    height: 85vh; /* 视口高度的85% */
    margin: 0 auto;
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  
  .mobile-pdf-link {
    display: none;
    text-align: center;
    margin-top: 1em;
    padding: 1em;
    background: #f8f8f8;
    border-radius: 8px;
  }
  
  .mobile-pdf-link a {
    color: #3a651d;
    font-weight: bold;
  }
  
  @media (max-width: 768px) {
    .mobile-pdf-link {
      display: block;
    }
  }
</style>
