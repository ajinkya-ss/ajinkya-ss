<style>
/* Make banner image full screen without affecting the rest of the page */
.banner-section {
  position: relative;
  width: 100vw;
  height: 100vh;
  overflow: hidden;
  margin: 0;
  padding: 0;
}

/* Banner image */
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
}

/* Scroll-down arrow */
.scroll-down {
  position: absolute;
  bottom: 10px;
  left: 50%;
  transform: translateX(-50%);
  color: white;
  font-size: 1em;
  text-decoration: none;
  cursor: pointer;
}

/* Ensure content below the banner displays normally */
#main-content {
  padding: 2rem 1rem;
  max-width: 1100px;
  margin: 0 auto;
}
</style>

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

<!-- Banner -->
<div class="banner-section">
  <img src="images/Quotefancy-2059690-3840x2160.jpg" alt="Banner" class="banner-full">
  <div class="banner-overlay">
    <h1 style="font-size: 2.5em; margin: 0;">Ajinkya Shingote</h1>
    <p style="font-size: 1.1em; margin: 5px 0 0;">Ph.D. Student · University of Notre Dame</p>
  </div>
  <a href="#main-content" class="scroll-down">▼</a>
</div>

<!-- Main content starts -->
<div id="main-content">
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
