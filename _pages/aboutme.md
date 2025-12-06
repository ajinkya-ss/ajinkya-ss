---
layout: single
title: "About Me"
permalink: /aboutme/
author_profile: true
classes: wide
---

<!-- Improve paragraph readability -->
<style>
.page__content p {
  line-height: 1.8;
}
</style>

<!-- Centered title WITHOUT shifting or clipping -->
<style>
.page__title,
h1.page__title,
h1 {
  text-align: center !important;
  margin-top: 20px !important;
  margin-bottom: 20px !important;
  font-size: 2rem !important;
  font-weight: 600 !important;
  position: static !important;  /* remove offset */
}
</style>

<!-- FIX CLIPPING + RESPONSIVE LAYOUT -->
<style>
/* Use natural flexbox layout from Minimal Mistakes */
.page__inner-wrap {
  display: flex;
  gap: 30px;
  max-width: 100% !important;
}

/* Sidebar (your author profile) */
.page__sidebar,
.author-profile {
  flex: 0 0 260px;        /* fixed width column */
  max-width: 260px;
}

/* MAIN CONTENT – grows without clipping */
.page__content {
  flex: 1 1 auto;
  min-width: 0 !important;          /* KEY FIX for Edge */
  overflow-wrap: break-word;
  word-break: break-word;
  padding-right: 10px !important;
}

/* Mobile layout */
@media (max-width: 768px) {
  .page__inner-wrap {
    flex-direction: column;
  }

  .page__sidebar,
  .author-profile {
    max-width: 100% !important;
    width: 100% !important;
  }
}
</style>
---

I am a second-year doctoral student in the Department of Materials Science and Engineering, working under the guidance of [**Professor Gregory Hartland**](https://sites.nd.edu/hartland-group/?page_id=5) at the [**University of Notre Dame**](https://www.nd.edu/). My research focuses on strong exciton–plasmon coupling in metal–semiconductor hybrid nanostructures. More broadly, I am interested in materials chemistry, with a particular emphasis on designing and understanding materials for energy-related applications.

Before starting my Ph.D., I earned a **BSMS** in Chemistry from the [**Indian Institute of Science Education and Research (IISER) Pune**](https://www.iiserpune.ac.in/), Maharashtra, India, where I completed my master’s project under the mentorship of [**Professor Angshuman Nag**](https://angshumaniiserpune.wixsite.com/grouppage).

---

### 🎓 Education

- **Ph.D.** [**Material Science and Engineering: Chemistry**, **University of Notre Dame**](https://mse.nd.edu/people/current-students/) (2024–Present)  
- **BS–MS**, [**IISER Pune**](https://www.iiserpune.ac.in/institute/people/students/?year=2024&degree=BSMS&department=0&alumni=False#Results)

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
