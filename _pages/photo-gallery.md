---
layout: page
title: "Photo Gallery"
permalink: /photo-gallery/
---

<style>
/* gallery CSS */
.photo-gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  justify-content: center;
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
}

.photo-item img:hover {
  transform: scale(1.05);
}
</style>

Here are photos of my kitty 🐾:

<div class="photo-gallery">
  {% for file in site.static_files %}
    {% assign path = file.path | downcase %}
    {% if path contains "assets/images/gallery/" %}
      <div class="photo-item">
        <a href="{{ '/assets/images/gallery/congruent_number.jpg'| relative_url }} ">
          < img src="{{ '/assets/images/gallery/congruent_number.jpg'| relative_url }}" alt="kitty photo" />
        </a >
      </div>
    {% endif %}
  {% endfor %}
</div>
