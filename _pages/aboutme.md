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
.page__title,
h1.page__title,
h1 {
  text-align: center !important;
  margin-top: 20px !important;
  margin-bottom: 20px !important;
  position: relative;
  left: -60px; /* adjust this value as needed */
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

/* mobile behaviour */
@media (max-width: 768px) {
  .page__content {
    margin-left: auto !important;
    width: 95% !important;
    padding-right: 0 !important;
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

I am a second-year doctoral student in the Department of Materials Science and Engineering, working under the guidance of [**Professor Gregory Hartland**](https://sites.nd.edu/hartland-group/?page_id=5) at the [**University of Notre Dame**](https://www.nd.edu/). My research focuses on strong exciton–plasmon coupling in metal–semiconductor hybrid nanostructures. More broadly, I am interested in materials chemistry, with a particular emphasis on designing and understanding materials for energy-related applications.
Before starting my Ph.D., I earned a **BSMS** in Chemistry from the [**Indian Institute of Science Education and Research (IISER) Pune**](https://www.iiserpune.ac.in/), Maharastra, India, where I completed my master’s project under the mentorship of [**Professor Angshuman Nag**](https://angshumaniiserpune.wixsite.com/grouppage).

---

### 🎓 Education

- **Ph.D.** [**Material Science and Engineering:Chemistry**, **University of Notre Dame**](https://mse.nd.edu/people/current-students/) (2024–Present)  
- **BS–MS**, [**IISER Pune**]([https://www.iiserpune.ac.in/](https://www.iiserpune.ac.in/institute/people/students/?year=2024&degree=BSMS&department=0&alumni=False#Results))

---

### 🔬 Research Interests

- Exciton–plasmon coupling  
- Nanomaterial design for optoelectronics  
- Ultrafast spectroscopy studies of single nanostructures

---

### 🌱 Outside the Lab

I enjoy exploring science communication, web design, and photography.

---

📫 **Contact:**  
- Email: ashingot@nd.edu  
- GitHub: [ajinkya-ss](https://github.com/ajinkya-ss)
