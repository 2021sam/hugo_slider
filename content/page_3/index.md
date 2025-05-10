+++
date = '2025-05-08T23:29:58-07:00'
draft = true
title = 'Page_3'
+++

<style>
  /* Splide.js Styles */
  .splide {
    max-width: 800px;
    margin: 2rem auto;
  }
  .splide__slide img {
    width: 100%;
    border-radius: 8px;
  }
</style>

<script>
  document.addEventListener('DOMContentLoaded', function () {
    new Splide('.splide', {
      type       : 'loop',
      perPage    : 1,
      autoplay   : true,
      interval   : 5000,
      arrows     : true,
      pagination: true,
    }).mount();
  });
</script>

## Introduction

Welcome to **Page_3**! Below is an image slider showcasing some of our featured images.

path:
/Users/2021sam/apps/BEAR/hugo/05_06/quickstart/content/posts/post_3/index.md

<div class="splide">
  <div class="splide__track">
    <ul class="splide__list">
      <li class="splide__slide">
        <img src="https://via.placeholder.com/800x400?text=Image+1" alt="Image 1">
      </li>
      <li class="splide__slide">
        <img src="https://via.placeholder.com/800x400?text=Image+2" alt="Image 2">
      </li>
      <li class="splide__slide">
        <img src="https://via.placeholder.com/800x400?text=Image+3" alt="Image 3">
      </li>
    </ul>
  </div>
</div>

Feel free to explore more content on our site!
