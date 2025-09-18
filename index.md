---
layout: home
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/lab-banner.jpg
  actions:
    - label: "View Publications"
      url: "/publications/"
    - label: "Download CV"
      url: "/cv/"
excerpt: "Biotechnologist specializing in nanotechnology, drug delivery systems, and therapeutic protein research"
intro: 
  - excerpt: "Welcome to my academic website. I'm a researcher passionate about developing innovative nanotherapeutic carriers and optimizing bioprocess systems for enhanced drug delivery."
feature_row:
  - image_path: /assets/images/nanoparticles.jpg
    alt: "nanotechnology research"
    title: "Nanotechnology & Drug Delivery"
    excerpt: "Developing carbon nanodots and nanocellulose systems for enhanced therapeutic protein bioavailability and targeted drug delivery applications."
  - image_path: /assets/images/cell-culture.jpg
    alt: "cell culture research"
    title: "Mammalian Cell Culture"
    excerpt: "Expertise in A549 cell line maintenance, bioprocess optimization, and GMP-aligned protocols for therapeutic applications."
  - image_path: /assets/images/bioprocess.jpg
    alt: "bioprocess optimization"
    title: "Bioprocess Optimization"
    excerpt: "Bioreactor operations, analytical biochemistry, and statistical analysis for industrial biotechnology applications."
---

{% include feature_row id="intro" type="center" %}

## Recent News & Achievements

- **September 2024**: Published research on fruit peel-derived carbon dots in *Chemistry Select*
- **May 2024**: Graduated with distinction from MSc Drug Design and Biomedical Science, Edinburgh Napier University
- **2024**: Completed research on nano silver and nano cellulose mediated responses in lung epithelial cells
- **2021**: Achieved distinction in MSc (Integrated) Biotechnology from Sardar Patel University

{% include feature_row %}

## Featured Photography

As a passionate photographer, I capture the beauty of science and nature. Here are some of my favorite shots:

<div class="photo-gallery">
  <div class="photo-item">
    <img src="/assets/images/photos/microscopy1.jpg" alt="Microscopy Art">
    <div class="photo-caption">Crystalline structures under polarized light</div>
  </div>
  <div class="photo-item">
    <img src="/assets/images/photos/nature1.jpg" alt="Edinburgh Landscape">
    <div class="photo-caption">Edinburgh's Royal Mile at sunset</div>
  </div>
  <div class="photo-item">
    <img src="/assets/images/photos/lab1.jpg" alt="Laboratory">
    <div class="photo-caption">Cell culture facility aesthetic</div>
  </div>
</div>

[View More Photography](/photography/){: .btn .btn--primary}

## Quick Links

- [Research Projects](/research/) - Explore my nanobiotechnology research
- [Publications](/publications/) - Peer-reviewed articles and presentations  
- [CV](/cv/) - Complete academic and professional background
- [Photography](/photography/) - My artistic perspective on science and nature

---

*"Innovation in biotechnology comes from bridging the gap between fundamental research and practical applications."*

<style>
.photo-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
  margin: 2rem 0;
}

.photo-item {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.photo-item img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  transition: transform 0.3s ease;
}

.photo-item:hover img {
  transform: scale(1.05);
}

.photo-caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0,0,0,0.8));
  color: white;
  padding: 1rem;
  font-size: 0.9rem;
}
</style>
