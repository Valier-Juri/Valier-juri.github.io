---
title: "Arts"
layout: page
permalink: /arts
---

<!-- CSS Styling -->
<style>
.art-section {
  margin-bottom: 4em;
}

.art-title {
  font-size: 1.4em;
  font-weight: 700;
  margin-bottom: 0.3em;
  color: #333;
}

.art-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5em;
}

.art-grid figure {
  width: 280px;
  aspect-ratio: 3 / 4; /* Ensures consistency */
  position: relative;
  overflow: hidden;
  border-radius: 10px;
  background-color: #f9f9f9;
  box-shadow: 0 4px 10px rgba(0,0,0,0.06);
  transition: transform 0.3s ease;
  cursor: zoom-in;
}

.art-grid figure:hover {
  transform: scale(1.02);
}

.art-grid img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: 0.3s ease;
}

.art-grid figcaption {
  font-size: 0.9em;
  text-align: center;
  color: #666;
  margin-top: 0.4em;
}

/* Fullscreen lightbox */
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

<!-- Lightbox Container -->
<div id="lightbox" class="lightbox-modal" onclick="this.classList.remove('active')">
  <img id="lightbox-img" src="">
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  document.querySelectorAll('.art-grid img').forEach(img => {
    img.addEventListener('click', () => {
      const lightbox = document.getElementById('lightbox');
      const lightboxImg = document.getElementById('lightbox-img');
      lightboxImg.src = img.src;
      lightbox.classList.add('active');
    });
  });
});
</script>

<!-- === Animated Manga === -->
<div class="art-section">
  <div class="art-title">Animated Manga</div>
  <p><em>Vivi</em> – A short manga loop originally designed as video with BGM, adapted here as a GIF preview.</p>
  <div class="art-grid">
    <figure>
      <img src="/assets/manga-animation.gif" alt="Animated Manga">
      <figcaption>Vivi</figcaption>
    </figure>
  </div>
</div>

<!-- === Illustration Storybook === -->
<div class="art-section">
  <div class="art-title">Illustration Storybook</div>
  <p><em>Kana</em> – A quiet narrative through light and gesture.</p>
  <div class="art-grid">
    <figure>
      <img src="/assets/illustration1.jpg" alt="Kana 1">
      <figcaption>Kana 1</figcaption>
    </figure>
  </div>
</div>

<!-- === Surrealism === -->
<div class="art-section">
  <div class="art-title">Surrealism</div>
  <p>A few introspective moments captured in dreams and distortions.</p>
  <div class="art-grid">
    <figure>
      <img src="/assets/illustration2.jpg" alt="Sistina">
      <figcaption>Sistina</figcaption>
    </figure>
  </div>
</div>



