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
    margin: 0; /* Add this line */
    min-height: 100vh;
  }

  .page-header {
    background-image: url('/Android_Feature_1024x500.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    height: 150px;
    overflow: hidden;
    position: fixed; /* Change this line from relative to fixed */
    top: 0; /* Add this line */
    left: 0; /* Add this line */
    width: 100%; /* Add this line */
    z-index: 1000; /* Add this line */
  }
  .page-header h1 {
    color: transparent;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .page-content {
    margin-top: 150px; /* Add this line */
    padding: 20px; /* Add this line */
  }
</style>

<div class="page-header">
  <h1>Welcome to my website!</h1>
</div>

<div class="page-content">
  This is the homepage of my GitHub Pages site using the Cayman theme.
</div>
