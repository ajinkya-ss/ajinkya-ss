---
permalink: /
title: "Welcome"
layout: default
author_profile: false
---

<style>
/* safe global reset for box-sizing only */
*, *::before, *::after { box-sizing: border-box; }

/* Banner (isolated, does not modify theme container or body) */
.banner-section {
  position: relative;
  width: 100%;
  height: 100vh;          /* full viewport height */
  overflow: hidden;
  margin: 0;
  padding: 0;
}

/* Keep banner image responsive within banner-section */
.banner-full {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* Overlay text at the bottom */
.banner-overlay {
  position: absolute;
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  text-align: center;
  background: rgba(0, 0, 0, 0.45);
  padding: 15px 30px;
  border-radius: 12px;
  max-width: 90vw;
  z-index: 2;
}

/* Scroll-down arrow positioned inside banner */
.scroll-down {
  position: absolute;
  bottom: 12px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  font-size: 1.2rem;
  text-decoration: none;
  cursor: pointer;
  z-index: 3;
  line-height: 1;
  padding: 6px 10px;
}

/* Main content: let theme container manage widths, but add padding for readability */
#main-content {
  padding: 2rem 1rem;
  margin: 0 auto;
  /* do not set max-width here if your theme already provides a container; it's safe to leave */
}

/* Quick Access card grid */
.quick-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  margin-top: 1rem;
}

/* Individual card: allow theme to control container; ensure cards behave consistently */
.quick-card {
  flex: 1 1 200px;
  max-width: 250px;
  text-align: center;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  text-decoration: none;
  display: block;
}

/* small visual tweaks for accessible focus/hover */
.quick-card:focus,
.quick-card:hover {
  transform: translateY(-4px);
  transition: transform 160ms ease;
}

/* Responsive: on very small screens let cards become full width */
@media (max-width: 420px) {
  .quick-card { flex: 1 1 100%; max-width: none; }
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
  const arrow = document.querySelector(".scroll-down");
  const target = document.querySelector("#main-content");

  if (arrow && target) {
    arrow.addEventListener("click", function(e){
      e.preventDefault();
      target.scrollIntoView({ behavior: "smooth" });
    });
  }
});
</script>

<!-- Banner -->
<div class="banner-section" aria-hidden="false">
  <img src="images/Quotefancy-2059690-3840x2160.jpg" alt="Banner" class="banner-full">
  <div class="banner-overlay" role="banner">
    <h1 style="font-size: 2.5em; margin: 0;">Ajinkya Shingote</h1>
    <p style="font-size: 1.05em; margin: 5px 0 0;">Ph.D. Student · University of Notre Dame</p>
  </div>
  <a href="#main-content" class="scroll-down" aria-label="Scroll to main content">▼</a>
</div>

<!-- Main content -->
<div id="main-content">
  <p>📫 <strong>You can contact me via:</strong></p>

  <ul>
    <li>📧 ashingot@nd.edu</li>
    <li>📧 ajinkya.shingote@students.iiserpune.ac.in</li>
  </ul>

  <hr style="margin-top: 2rem;">

  <h2 style="text-align: center;">🔗 Quick Access</h2>

  <div class="quick-grid" role="navigation" aria-label="Quick links">
    <a class="quick-card" href="//publications/" style="background-color: #e6f4ea; color:#14532d;">
      <h3>📚 Publications</h3>
      <p style="font-size: 0.9em;">Explore my peer-reviewed articles and academic output.</p>
    </a>

    <a class="quick-card" href="//files/CV.pdf" style="background-color: #e6f0fa; color:#003366;">
      <h3>📄 CV</h3>
      <p style="font-size: 0.9em;">Get an overview of my academic and research experience.</p>
    </a>

    <a class="quick-card" href="//project/" style="background-color: #fff4e6; color:#cc6600;">
      <h3>🧠 Projects</h3>
      <p style="font-size: 0.9em;">Discover my research, academic, and personal projects.</p>
    </a>

    <a class="quick-card" href="//teaching/" style="background-color: #fffde6; color:#997a00;">
      <h3>📘 Teaching</h3>
      <p style="font-size: 0.9em;">Courses I have assisted or instructed.</p>
    </a>

    <a class="quick-card" href="//year-archive/" style="background-color: #f3e6fa; color:#663399;">
      <h3>🏆 Awards</h3>
      <p style="font-size: 0.9em;">Learn about my interests and life outside PhD work!</p>
    </a>
  </div>
</div>
