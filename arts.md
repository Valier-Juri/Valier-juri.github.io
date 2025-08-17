---
title: "Arts"
layout: page
permalink: /arts
---

<div class="art-intro">
  <p>艺术创作是我表达思想和情感的方式。这些作品展示了我对动漫、插画和数字艺术的热爱，灵感来源于我的旅行经历、记忆和想象。</p>
</div>

<style>
.art-intro {
  margin-bottom: 2.5em;
  padding-bottom: 1.5em;
  border-bottom: 1px solid rgba(169, 132, 103, 0.2);
  font-size: 1.05em;
  line-height: 1.7;
}

.art-section {
  margin-bottom: 5em;
}

.art-title {
  font-family: "Playfair Display", Georgia, serif;
  font-size: 1.8em;
  font-weight: 600;
  margin-bottom: 1em;
  color: #4A4A4A;
  position: relative;
  padding-bottom: 0.5em;
}

.art-title::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 60px;
  height: 3px;
  background-color: #A98467;
}

.masonry-grid {
  column-count: 3;
  column-gap: 2em;
}

@media (max-width: 900px) {
  .masonry-grid {
    column-count: 2;
  }
}

@media (max-width: 600px) {
  .masonry-grid {
    column-count: 1;
  }
}

.masonry-grid figure {
  display: inline-block;
  width: 100%;
  margin: 0 0 2em;
  break-inside: avoid;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  transition: all 0.4s ease;
  cursor: zoom-in;
  position: relative;
}

.masonry-grid figure::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(169, 132, 103, 0.2);
  opacity: 0;
  transition: opacity 0.4s ease;
  z-index: 1;
}

.masonry-grid figure:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.12);
}

.masonry-grid figure:hover::before {
  opacity: 1;
}

.masonry-grid img {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.5s ease;
  filter: saturate(0.95);
}

.masonry-grid figure:hover img {
  transform: scale(1.03);
}

.masonry-grid figcaption {
  text-align: center;
  padding: 0.8em 1em;
  font-size: 1em;
  color: #4A4A4A;
  font-family: "Playfair Display", Georgia, serif;
  border-top: 1px solid rgba(169, 132, 103, 0.1);
  background-color: rgba(255, 255, 255, 0.9);
  position: relative;
  z-index: 2;
}

/* Lightbox for zoom */
.lightbox-modal {
  display: none;
  position: fixed;
  z-index: 1000;
  inset: 0;
  background: rgba(0, 0, 0, 0.85);
  justify-content: center;
  align-items: center;
  backdrop-filter: blur(5px);
  transition: opacity 0.3s ease;
}

.lightbox-modal img {
  max-height: 90vh;
  max-width: 90vw;
  border-radius: 12px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
  transform: scale(0.95);
  opacity: 0;
  transition: transform 0.4s ease, opacity 0.4s ease;
}

.lightbox-modal.active {
  display: flex;
}

.lightbox-modal.active img {
  transform: scale(1);
  opacity: 1;
}
</style>

<!-- Lightbox functionality -->
<div id="lightbox" class="lightbox-modal" onclick="this.classList.remove('active')">
  <img id="lightbox-img" src="">
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  document.querySelectorAll('.masonry-grid img').forEach(img => {
    img.addEventListener('click', () => {
      const lightbox = document.getElementById('lightbox');
      const lightboxImg = document.getElementById('lightbox-img');
      lightboxImg.src = img.src;
      lightbox.classList.add('active');
      
      // Add animation effect when opening lightbox
      setTimeout(() => {
        lightboxImg.style.opacity = '1';
        lightboxImg.style.transform = 'scale(1)';
      }, 10);
    });
  });
  
  // Close lightbox on ESC key
  document.addEventListener('keydown', (e) => {
    if (e.key === 'Escape') {
      const lightbox = document.getElementById('lightbox');
      if (lightbox.classList.contains('active')) {
        const lightboxImg = document.getElementById('lightbox-img');
        lightboxImg.style.opacity = '0';
        lightboxImg.style.transform = 'scale(0.95)';
        
        setTimeout(() => {
          lightbox.classList.remove('active');
        }, 300);
      }
    }
  });
});
</script>

<!-- === Featured Animated Manga === -->
<div class="art-section">
  <h2 class="art-title">动漫创作</h2>
  <div class="masonry-grid">
    <figure>
      <img src="/assets/manga-animation.gif" alt="Vivi">
      <figcaption>Vivi - 原创角色动画</figcaption>
    </figure>
  </div>
</div>

<!-- === Sequential and Themed Artworks === -->
<div class="art-section">
  <h2 class="art-title">插画作品</h2>
  <div class="masonry-grid">
    <figure>
      <img src="/assets/illustration1.jpg" alt="Kana 1">
      <figcaption>Kana - 水彩风格数字插画</figcaption>
    </figure>
    <figure>
      <img src="/assets/illustration2.jpg" alt="Sistina">
      <figcaption>Sistina - 角色设计</figcaption>
    </figure>
    <figure>
      <img src="/assets/your-photo.jpg" alt="Landscape">
      <figcaption>风景写生</figcaption>
    </figure>
  </div>
</div>

<!-- === Photography === -->
<div class="art-section">
  <h2 class="art-title">摄影作品</h2>
  <div class="masonry-grid">
    <figure>
      <img src="/assets/IMG_1574.JPG" alt="Photography 1">
      <figcaption>自然光影</figcaption>
    </figure>
  </div>
</div>
