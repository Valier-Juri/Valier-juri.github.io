---
title: "Arts"
layout: page
permalink: /arts
---

<style>
.art-section {
  margin-bottom: 4em;
}

.art-title {
  font-size: 1.5em;
  font-weight: 700;
  margin-bottom: 0.8em;
}

.masonry-grid {
  column-count: 3;
  column-gap: 1.5em;
}

.masonry-grid figure {
  display: inline-block;
  width: 100%;
  margin: 0 0 1.5em;
  break-inside: avoid;
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.06);
  overflow: hidden;
  transition: transform 0.3s ease;
  cursor: zoom-in;
}

.masonry-grid img {
  width: 100%;
  height: auto;
  display: block;
  border-bottom: 1px solid #eee;
}

.masonry-grid figcaption {
  text-align: center;
  padding: 0.5em 0.8em;
  font-size: 0.95em;
  color: #444;
}

/* Lightbox for zoom */
.lightbox-modal {
  display: none;
  position: fixed;
  z-index: 1000;
  inset: 0;
  background: rgba(0, 0, 0, 0.9);
  justify-content: center;
  align-items: center;
}
.lightbox-modal img {
  max-height: 90vh;
  max-width: 90vw;
  border-radius: 10px;
}
.lightbox-modal.active {
  display: flex;
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
    });
  });
});
</script>

<!-- === Featured Animated Manga === -->
<div class="art-section">
  <div class="art-title">Animated Manga</div>
  <div class="masonry-grid">
    <figure>
      <img src="/assets/manga-animation.gif" alt="Vivi">
      <figcaption>Vivi</figcaption>
    </figure>
  </div>
</div>

<!-- === Sequential and Themed Artworks === -->
<div class="art-section">
  <div class="art-title">Artworks</div>
  <div class="masonry-grid">
    <figure>
      <img src="/assets/illustration1.jpg" alt="Kana 1">
      <figcaption>Kana 1</figcaption>
    </figure>
    <figure>
      <img src="/assets/illustration2.jpg" alt="Sistina">
      <figcaption>Sistina</figcaption>
    </figure>
    <figure>
      <img src="/assets/manga1.jpg" alt="Manga Page 1">
      <figcaption>Manga Page 1</figcaption>
    </figure>
    <figure>
      <img src="/assets/girl1.jpg" alt="Girl 1">
      <figcaption>Girl 1</figcaption>
    </figure>
    <figure>
      <img src="/assets/girl2.jpg" alt="Girl 2">
      <figcaption>Girl 2</figcaption>
    </figure>
    <figure>
      <img src="/assets/manga2.jpg" alt="Manga Page 2">
      <figcaption>Manga Page 2</figcaption>
    </figure>
  </div>
</div>
