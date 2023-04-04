---
layout: default
title: JUMP ROPE FOREVER
---

<style>
  body {
    background-image: url('/AppFeatures.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    margin: 0;
    min-height: 100vh;
  }

  .page-header {
    background-image: url('/Android_Feature_1024x500.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    height: 150px;
    overflow: hidden;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
    transition: height 0.3s;
  }
  .page-header h1 {
    color: transparent;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .page-content {
    margin-top: 150px;
    padding: 20px;
    min-height: 100vh; /* Add this line */
  }
</style>

<div class="page-header">
  <h1>Welcome to my website!</h1>
</div>

<div class="page-content">
  This is the homepage of my GitHub Pages site using the Cayman theme.
</div>

<script>
  window.addEventListener('scroll', function() {
    var header = document.querySelector('.page-header');
    var scrollPos = window.scrollY;
    var headerHeight = Math.max(150 - scrollPos * 0.5, 50);

    header.style.height = headerHeight + 'px';
  });
</script>
