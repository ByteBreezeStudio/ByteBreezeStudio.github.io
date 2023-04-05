---
layout: default
---

<style>
.header-wrapper {
  position: fixed;
  width: 100%;
  background-image: url('/Android_Feature_1024x500.png');
  background-size: cover;
  background-position: center;
  z-index: 1;
  transition: all 0.3s ease;
}

.body-wrapper {
  margin-top: 100px; /* Adjust this value based on your header height */
  background-image: url('AppFeatures.jpg');
  background-size: cover;
  background-position: center;
  min-height: 100vh;
  z-index: 0;
}

.content {
  padding: 2rem;
}
</style>

<div class="header-wrapper">
  <header class="masthead clearfix">
    <div class="inner">
      <h3 class="masthead-brand">{{ site.title }}</h3>
      <nav class="nav nav-masthead">
        {% for link in site.navigation %}
          <a class="nav-link {% if page.url == link.url %}active{% endif %}" href="{{ link.url }}">{{ link.title }}</a>
        {% endfor %}
      </nav>
    </div>
  </header>
</div>

<div class="body-wrapper">
  <main class="content" role="main">
    <!-- Your content goes here -->
  </main>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const header = document.querySelector(".header-wrapper");
  const initialHeight = header.clientHeight;

  window.addEventListener("scroll", () => {
    const scrollValue = window.scrollY;
    header.style.height = initialHeight - scrollValue + "px";
  });
});
</script>
