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
    min-height: 100vh;
  }

  .page-header {
    background-image: url('/Android_Feature_1024x500.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    height: 150px; /* Updated this line */
    overflow: hidden;
    position: relative; /* Add this line */
  }
  .page-header h1 {
    color: transparent;
    position: absolute; /* Add this line */
    top: 50%; /* Add this line */
    left: 50%; /* Add this line */
    transform: translate(-50%, -50%); /* Add this line */
  }
</style>

<div class="page-content">
  This is the homepage of my GitHub Pages site using the Cayman theme.
</div>

<script>
  window.addEventListener('scroll', function() {
    var header = document.querySelector('.page-header');
    var body = document.querySelector('.page-content');
    var scrollPos = window.scrollY;
    var headerHeight = Math.max(150 - scrollPos, 50);

    header.style.height = headerHeight + 'px';
    body.style.marginTop = headerHeight + 'px';
  });
</script>
