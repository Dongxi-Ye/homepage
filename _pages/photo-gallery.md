---
layout: page
title: "Photo Gallery"
permalink: /photo-gallery/
---

<style>
/* --- Simple responsive photo grid styling --- */
.photo-gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
  margin-top: 20px;
}

.photo-item {
  flex: 1 0 200px;
  max-width: 250px;
  overflow: hidden;
}

.photo-item img {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-radius: 4px;
  transition: transform 0.3s ease;
  box-shadow: 0 2px 6px rgba(0,0,0,0.15);
}

.photo-item img:hover {
  transform: scale(1.05);
}
</style>

Here are some photos of my kitty 🐾:

<div class="photo-gallery">
  <div class="photo-item">
    <a href=" '/assets/images/gallery/congruent_number.jpg' | relative_url }}">
      < img src="{{ '/assets/images/gallery/congruent_number.jpg' | relative_url }}" alt="kitty photo" />
    </a >
  </div>
</div>
