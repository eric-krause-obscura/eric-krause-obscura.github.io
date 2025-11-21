---
layout: splash
title: "Eric Krause Obscura"
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "/assets/images/Reaching.jpg"
  caption: "Reaching"
excerpt: "Exploring the surreal in the mundane — moments when reality thins and the other world bleeds through."
feature_row:
  - image_path: /assets/images/Symbol.jpg
    title: "Symbol"
    excerpt: "**Next to the Symbol...**"
    url: "/TheThinPlaces/Symbol"
    btn_label: "Symbol"
    btn_class: "btn--primary"
  - image_path: /assets/images/The%20Tower.jpg
    title: "The Tower"
    excerpt: "**Out of the fog...**"
    url: "/TheThinPlaces/TheTower"
    btn_label: "The Tower"
    btn_class: "btn--primary"
  - image_path: /assets/images/Nest.jpg
    title: "Nest"
    excerpt: "**Something...**"
    url: "/TheThinPlaces/Nest"
    btn_label: "Nest"
    btn_class: "btn--primary"
  - image_path: /assets/images/The%20Heavenly%20Ceiling.jpg
    title: "The Heavenly Ceiling"
    excerpt: "**The heavens...**"
    url: "/TheThinPlaces/TheHeavenlyCeiling"
    btn_label: "The Heavenly Ceiling"
    btn_class: "btn--primary"
  - image_path: /assets/images/Wound.jpg
    title: "Wound"
    excerpt: "**A gash appeared...**"
    url: "/TheThinPlaces/Wound"
    btn_label: "Wound"
    btn_class: "btn--primary"
  - image_path: /assets/images/Stain.jpg
    title: "Stain"
    excerpt: "**This was...**"
    url: "/TheThinPlaces/Stain"
    btn_label: "Stain"
    btn_class: "btn--primary"
---

{% include feature_row %}

<script>
document.addEventListener("DOMContentLoaded", function() {
  const features = Array.from(document.querySelectorAll(".feature__item"));
  if (features.length === 0) return;

  const showCount = 3; // ← change this number (e.g. 3, 6, etc.)
  const shuffled = features.sort(() => 0.5 - Math.random());
  const selected = shuffled.slice(0, showCount);

  const container = features[0].parentNode;
  container.innerHTML = "";
  selected.forEach(el => container.appendChild(el));
});
</script>
