---
title: "Research Interests"
collection: portfolio
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
---
Broadly, I am interested in materials chemistry and optical spectroscopy, with a particular focus on designing materials for energy-related applications and probing their functionalities using custom-built optical characterization techniques. My current work focuses on probing strong exciton–plasmon coupling in metal–semiconductor hybrid structures via optical spectroscopy.
Efficient routing of energy in ultrathin materials and devices is essential for advancing solar and optoelectronic technologies, and metal–semiconductor nanostructures lie at the center of this effort. Coupling localized surface plasmon in metal with exciton in semiconductor offers a powerful platform for modifying energy landscape and directing energy transport at the nanoscale. This hybridization leads to the formation of exciton–plasmon polaritons, quasiparticles that inherit properties from both light and matter. As a consequence, these coupled states have already been explored for optical switching, nonlinear optics and low threshold nanolasing, underscoring their broad technological relevance. However, experimentally visualizing these coupled states is challenging, requiring advanced optical microscopy and spectroscopic techniques. In my work, we will characterize these hybrid states using spatial modulation spectroscopy and transient absorption microscopy. Spatial modulation spectroscopy will provide spectroscopic signatures of the states by measuring the absolute extinction of individual nanostructures with high sensitivity while transient absorption microscopy will enable time-resolved mapping of exciton–polariton diffusion. Together, these measurements will offer a comprehensive understanding of the formation, dynamics, and transport properties of the coupled states, offering insight into how engineered nanostructures could channel energy more efficiently in solar energy conversion devices.
