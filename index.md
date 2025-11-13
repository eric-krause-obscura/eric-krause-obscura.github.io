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
    alt: "Symbol"
    title: "Symbol"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/The%20Tower.jpg
    alt: "The Tower"
    title: "The Tower"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/Nest.jpg
    title: "Nest"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/The%Heavenly%Ceiling.jpg
    title: "The Heavenly Ceiling"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/Wound.jpg
    title: "Wound"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: /assets/images/Stain.jpg
    title: "Stain"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
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
