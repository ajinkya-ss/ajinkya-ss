---
layout: single
title: "About Me"
permalink: /aboutme/
author_profile: true
classes: wide
---
<style>
.page__content p {
  line-height: 1.8; /* default ~1.4, so 1.8 gives more breathing room */
}
</style>

<style>
/* Education table: use the page's text size (theme tables default to 0.75em)
   and give every row the same column widths */
.page__content table.education-table {
  font-size: inherit;
  table-layout: fixed;
  width: 100%;
}
.page__content table.education-table td:first-child { width: 65%; }
.page__content table.education-table td:last-child  { width: 35%; }

/* phones: stack each row so the degree and advisor each get the full width */
@media (max-width: 37.5em) {
  .page__content table.education-table,
  .page__content table.education-table tbody,
  .page__content table.education-table tr,
  .page__content table.education-table td { display: block; width: 100% !important; }
  .page__content table.education-table td { border-right: 0; }
  .page__content table.education-table td:first-child { border-bottom: 0; padding-bottom: 0; }
}
</style>

<style>
.page__title,
h1.page__title,
h1 {
  text-align: center !important;
  margin-top: 20px !important;
  margin-bottom: 20px !important;
  position: relative;
  left: -210px; /* adjust this value as needed */
  font-size: 2rem !important;
  font-weight: 600 !important;
}
</style>

<style>
/* make sure parent wrappers can expand */
.page, .page__inner-wrap, .layout--single .page__inner-wrap {
  max-width: 100% !important;
  width: 100% !important;
}

/* initial safe defaults to avoid overlap while JS runs */
.page__content {
  margin-left: 200px !important;
  margin-right: 0 !important;
  width: calc(100% - 02px) !important;
  max-width: 100% !important;
  padding-right: 0px !important;
  box-sizing: border-box !important;
}

/* mobile and tablet behaviour: below 57.8125em (925px) the theme stacks the
   sidebar above the content, so drop the side offsets */
@media (max-width: 57.8em) {
  .page__content {
    margin-left: auto !important;
    width: 95% !important;
    padding-right: 0 !important;
  }
  .page__title,
  h1.page__title,
  h1 {
    left: 0 !important;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function () {
  // find the author/profile sidebar element (common possible selectors)
  const sidebarSelectors = [
    '.author-profile',      // some themes
    '.page__sidebar',
    '.sidebar',
    '.site-sidebar',
    '.author'
  ];
  let sidebar = null;
  for (const sel of sidebarSelectors) {
    const el = document.querySelector(sel);
    if (el) { sidebar = el; break; }
  }

  // if no sidebar found, nothing to do
  if (!sidebar) return;

  // compute effective width including margins
  const rect = sidebar.getBoundingClientRect();
  const style = window.getComputedStyle(sidebar);
  const marginLeft = parseFloat(style.marginLeft) || 0;
  const marginRight = parseFloat(style.marginRight) || 0;
  const effectiveWidth = Math.ceil(rect.width + marginLeft + marginRight);

  // apply to main content and parent wrappers
  const content = document.querySelector('.page__content') || document.querySelector('.content') || document.querySelector('main');
  const parentWraps = [
    document.querySelector('.page'),
    document.querySelector('.page__inner-wrap'),
    document.querySelector('.layout--single .page__inner-wrap')
  ].filter(Boolean);

  if (content) {
    content.style.marginLeft = effectiveWidth + 'px';
    content.style.marginRight = '0';
    content.style.width = 'calc(100% - ' + (effectiveWidth + 20) + 'px)'; // leave small gap
    content.style.maxWidth = '100%';
    content.style.boxSizing = 'border-box';
  }

  parentWraps.forEach(p => {
    p.style.maxWidth = '100%';
    p.style.width = '100%';
  });

  // Re-run on resize (debounced)
  let t;
  window.addEventListener('resize', function() {
    clearTimeout(t);
    t = setTimeout(function(){
      const rect2 = sidebar.getBoundingClientRect();
      const style2 = window.getComputedStyle(sidebar);
      const eff = Math.ceil(rect2.width + (parseFloat(style2.marginLeft)||0) + (parseFloat(style2.marginRight)||0));
      if (content) {
        content.style.marginLeft = eff + 'px';
        content.style.width = 'calc(100% - ' + (eff + 20) + 'px)';
      }
    }, 120);
  });
});
</script>


---

I am a Ph.D. candidate in Physical & Materials Chemistry at the [**University of Notre Dame**](https://www.nd.edu/), working under the guidance of [**Professor Gregory Hartland**](https://sites.nd.edu/hartland-group/?page_id=5). My research investigates nanoscale light–matter interactions using single-particle optical spectroscopy, with the goal of establishing fundamental design principles for next-generation optoelectronic devices. I currently study exciton–plasmon coupling in metal–semiconductor hybrid nanostructures using a custom-built Fourier-space optical imaging setup, complemented by electromagnetic simulations in COMSOL Multiphysics.
Before starting my Ph.D., I earned my B.S. and M.S. in Chemistry from the [**Indian Institute of Science Education and Research (IISER) Pune**](https://www.iiserpune.ac.in/), Maharashtra, India, where I completed my master’s project under the mentorship of [**Professor Angshuman Nag**](https://angshumaniiserpune.wixsite.com/grouppage). At IISER Pune, my research focused on luminescent halide perovskites, from short-wave infrared (SWIR) emitting double perovskites to the structure and exciton dynamics of layered hybrid perovskites.


---

### 🎓 Education

| **Ph.D., Chemistry**, [**University of Notre Dame**](https://www.nd.edu/) (2024–2029, expected) | Advisor: Prof. Gregory Hartland |
| **M.S., Chemistry**, [**IISER Pune**](https://www.iiserpune.ac.in/) (2023–2024) | Advisor: Prof. Angshuman Nag |
| **B.S., Chemistry**, [**IISER Pune**](https://www.iiserpune.ac.in/) (2019–2023) | Advisor: Prof. Pramod Pillai |
{: .education-table}

---

### 🔬 Research Interests

- Exciton–plasmon coupling in hybrid nanostructures
- Single-particle optical spectroscopy and Microscopy
- Ultrafast spectroscopy studies of single nanostructures
- Electromagnetic simulations of light–matter interactions (COMSOL Multiphysics)
- Luminescent halide perovskites for optoelectronic devices

---

### 🌱 Outside the Lab

When I'm not in the lab, you'll find me juggling, bowling, or working out at the gym. I also enjoy reading books on psychology and personal development, watching documentaries, vibe coding, and photography.

---

📫 **Contact:**  
- Email: ashingot@nd.edu  
- Office: 159 Stepan Chemistry, University of Notre Dame  
- GitHub: [ajinkya-ss](https://github.com/ajinkya-ss)
