---
permalink: /
title: "Welcome"
layout: default
author_profile: false
---

<!-- ========================== -->
<!-- Full-width, full-screen banner -->
<!-- ========================== -->

<style>
/* Remove default container margins for full-width homepage */
body, .container {
  margin: 0 !important;
  padding: 0 !important;
  max-width: 100% !important;
  width: 100% !important;
}

/* Make banner image cover full viewport */
.banner-full {
  width: 100vw;
  height: 100vh;
  object-fit: cover;
  display: block;
  margin: 0;
  padding: 0;
}

/* Optional: scroll-down arrow style */
.scroll-down {
  position: absolute;
  bottom: 30px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  font-size: 2em;
  text-decoration: none;
  cursor: pointer;
}
</style>

<!-- ========================== -->
<!-- Smooth scroll JS -->
<!-- ========================== -->
<script>
document.addEventListener("DOMContentLoaded", function() {
  const arrow = document.querySelector(".scroll-down");
  const target = document.querySelector("#main-content");

  if(arrow && target){
    arrow.addEventListener("click", function(e){
      e.preventDefault();
      target.scrollIntoView({ behavior: "smooth" });
    });
  }
});
</script>

<div style="position: relative; width: 100vw; height: 100vh; overflow: hidden;">
  <img src="image/banner.jpg" alt="Banner" class="banner-full">
  
  <!-- Optional overlay text -->
  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);
              color: white; text-align: center; background: rgba(0, 0, 0, 0.45);
              padding: 20px 40px; border-radius: 12px;">
    <h1 style="font-size: 2.8em; margin: 0;">Ajinkya Shingote</h1>
    <p style="font-size: 1.2em; margin: 10px 0 0;">Ph.D. Student · University of Notre Dame</p>
  </div>
  
  <!-- Scroll-down arrow -->
  <a href="#main-content" class="scroll-down">▼</a>
</div>



📫 **You can contact me via:**

- 📧 ashingot@nd.edu  
- 📧 ajinkya.shingote@students.iiserpune.ac.in  

<hr style="margin-top: 2rem;">

<h2 style="text-align: center;">🔗 Quick Access</h2>

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 20px; margin-top: 1rem;">

  <a href="publications/" style="flex: 1 1 200px; max-width: 250px; text-align: center; padding: 20px; border-radius: 12px; background-color: #e6f4ea; box-shadow: 0 4px 8px rgba(0,0,0,0.1); text-decoration: none; color: #14532d;">
  <h3>📚 Publications</h3>
  <p style="font-size: 0.9em;">Explore my peer-reviewed articles and academic output.</p>
  </a>

  <a href="files/CV.pdf" style="flex: 1 1 200px; max-width: 250px; text-align: center; padding: 20px; border-radius: 12px; background-color: #e6f0fa; box-shadow: 0 4px 8px rgba(0,0,0,0.1); text-decoration: none; color: #003366;">
    <h3>📄 CV</h3>
    <p style="font-size: 0.9em;">Get an overview of my academic and research experience.</p>
  </a>
    
  <a href="project/" style="flex: 1 1 200px; max-width: 250px; text-align: center; padding: 20px; border-radius: 12px; background-color: #fff4e6; box-shadow: 0 4px 8px rgba(0,0,0,0.1); text-decoration: none; color: #cc6600;">
    <h3>🧠 Projects</h3>
    <p style="font-size: 0.9em;">Discover my research, academic, and personal projects.</p>
  </a>

  <a href="teaching/" style="flex: 1 1 200px; max-width: 250px; text-align: center; padding: 20px; border-radius: 12px; background-color: #fffde6; box-shadow: 0 4px 8px rgba(0,0,0,0.1); text-decoration: none; color: #997a00;">
    <h3>📘 Teaching</h3>
    <p style="font-size: 0.9em;">Courses I have assisted or instructed.</p>
  </a>

  <a href="year-archive/" style="flex: 1 1 200px; max-width: 250px; text-align: center; padding: 20px; border-radius: 12px; background-color: #f3e6fa; box-shadow: 0 4px 8px rgba(0,0,0,0.1); text-decoration: none; color: #663399;">
    <h3>🏆 Awards</h3>
    <p style="font-size: 0.9em;">Learn about my interests and life outside PhD work!</p>
  </a>

</div>
</div>
