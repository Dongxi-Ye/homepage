---
layout: page
title: "Photo Gallery"
permalink: /photo-gallery/
---

Here are photos of my kitty:

<div class="photo-gallery">
  {% for file in site.static_files %}
    {% assign path = file.path | downcase %}
    {% if path contains "assets/images/gallery/" %}
      <div class="photo-item">
        <a href=" " data-lightbox="gallery">
          < img src="{{ file.path | relative_url }}" alt="kitty photo" />
        </a >
      </div>
    {% endif %}
  {% endfor %}
</div>
