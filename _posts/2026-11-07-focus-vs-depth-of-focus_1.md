---
title: 'Focus Tight or Focus Deep: Focal Length vs. Depth of Focus'
date: 2026-11-07
permalink: /posts/2026/11/focus-vs-depth-of-focus/
tags:
  - Gaussian beams
  - Optics essential
  - Focusing
---

When you focus a laser beam with a lens, the focal length decides two things at once: how small the spot gets, and how long the beam stays that small. I built an interactive poster to show this trade-off with the help of Claude. Change the focal length, beam diameter, or wavelength, and both diagrams update live.

<p style="text-align: center; margin: 1.5em 0;">
  <a href="{{ site.baseurl }}/files/focus-depth_1.html" target="_blank" rel="noopener">
    <img src="{{ site.baseurl }}/images/focus-depth-preview_1.png"
         alt="Interactive poster comparing the focus of a 150 mm and a 250 mm lens"
         style="width: 100%; border-radius: 8px;" />
  </a>
  <br>
  <a href="{{ site.baseurl }}/files/focus-depth_1.html" target="_blank" rel="noopener"><strong>Open the interactive poster →</strong></a>
</p>

Key equations
======

For a Gaussian beam of diameter *D* and wavelength *λ*, focused by a lens with focal length *f*:

* Spot diameter: **2w₀ = 4λf / (πD)**
* Rayleigh range: **z<sub>R</sub> = πw₀² / λ**
* Depth of focus: **DOF = 2z<sub>R</sub> = 8λf² / (πD²)**

Takeaway
======

The spot size grows with *f*, but the depth of focus grows with *f²*.

* **Short focal length:** tight spot and high intensity, but a short depth of focus, so alignment is sensitive.
* **Long focal length:** bigger spot, but a long depth of focus, so alignment is forgiving.

If you halve the focal length, the spot becomes half as big and the depth of focus becomes a quarter as long.
