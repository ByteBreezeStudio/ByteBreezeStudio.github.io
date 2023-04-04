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
    padding: 150px 0;
    margin-bottom: 50px;
    height: 150px; /* Add this line */
    overflow: hidden; /* Add this line */
  }
  .page-header h1 {
    color: transparent;
  }
</style>

<div class="page-header">
  <h1>Welcome to my website!</h1>
</div>

<div class="page-content"> <!-- Add this line -->
  This is the homepage of my GitHub Pages site using the Cayman theme.
</div> <!-- Add this line -->

<script> // Add the following JavaScript code
  window.addEventListener('scroll', function() {
    var header = document.querySelector('.page-header');
    var body = document.querySelector('.page-content');
    var scrollPos = window.scrollY;
    var headerHeight = Math.max(150 - scrollPos, 50);

    header.style.height = headerHeight + 'px';
    body.style.marginTop = headerHeight + 'px';
  });
</script>
