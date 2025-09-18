---
permalink: /publications/
title: "Publications"
author_profile: true
classes: wide
header:
  overlay_color: "#1a1a2e"
  overlay_filter: "1"
  overlay_image: /assets/images/fluorescent-vials-banner.jpg
---

<style>
/* Smooth Animations and Transitions */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideInLeft {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideInRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}

/* Container with gradient background */
.publications-wrapper {
  background: linear-gradient(135deg, 
    rgba(240, 248, 255, 0.95) 0%,
    rgba(230, 245, 255, 0.8) 25%,
    rgba(255, 250, 240, 0.95) 50%,
    rgba(245, 255, 245, 0.8) 75%,
    rgba(248, 240, 255, 0.95) 100%
  );
  padding: 2rem;
  border-radius: 20px;
  margin: 0 auto;
  max-width: 1000px;
  animation: fadeInUp 0.8s ease-out;
}

/* Animated Section Titles */
.section-title {
  position: relative;
  color: #2c3e50;
  font-size: 1.8rem;
  font-weight: 700;
  text-align: center;
  margin: 2rem 0;
  animation: slideInLeft 1s ease-out;
}

.section-title::before {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 4px;
  background: linear-gradient(45deg, #667eea, #764ba2);
  border-radius: 2px;
  animation: slideInRight 1.2s ease-out;
}

/* Publication Card with Hover Effects */
.publication-card {
  background: rgba(255, 255, 255, 0.98);
  border-radius: 20px;
  padding: 2.5rem;
  margin: 2rem 0;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08);
  border: 1px solid rgba(255, 255, 255, 0.3);
  backdrop-filter: blur(15px);
  transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  animation: fadeInUp 1.2s ease-out;
  position: relative;
  overflow: hidden;
}

.publication-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, #667eea, #764ba2, #f093fb);
  transition: left 0.6s ease;
}

.publication-card:hover::before {
  left: 0;
}

.publication-card:hover {
  transform: translateY(-8px) scale(1.02);
  box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
}

/* Year Badge with Animation */
.year-badge {
  background: linear-gradient(45deg, #667eea, #764ba2);
  color: white;
  padding: 0.6rem 1.5rem;
  border-radius: 30px;
  font-weight: 700;
  font-size: 0.9rem;
  display: inline-block;
  margin-bottom: 1.5rem;
  animation: float 3s ease-in-out infinite;
  box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
}

/* Title with Hover Effect */
.publication-title {
  margin: 1.5rem 0;
  font-size: 1.3rem;
  line-height: 1.4;
  font-weight: 600;
  transition: all 0.3s ease;
}

.publication-title a {
  color: #2c3e50;
  text-decoration: none;
  position: relative;
  transition: color 0.3s ease;
}

.publication-title a::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 2px;
  background: linear-gradient(45deg, #667eea, #764ba2);
  transition: width 0.4s ease;
}

.publication-title a:hover {
  color: #667eea;
}

.publication-title a:hover::after {
  width: 100%;
}

/* Authors with Stagger Animation */
.authors {
  color: #555;
  font-size: 1rem;
  margin: 1rem 0;
  line-height: 1.5;
  animation: slideInLeft 1.4s ease-out;
}

.journal-info {
  color: #666;
  font-size: 0.9rem;
  margin-bottom: 1.5rem;
  animation: slideInRight 1.6s ease-out;
}

/* Abstract Section with Animation */
.abstract-section {
  background: linear-gradient(135deg, 
    rgba(247, 250, 252, 0.9), 
    rgba(240, 248, 255, 0.9)
  );
  padding: 2rem;
  border-radius: 16px;
  margin: 2rem 0;
  border-left: 5px solid #667eea;
  backdrop-filter: blur(10px);
  animation: fadeInUp 2s ease-out;
  transition: all 0.3s ease;
}

.abstract-section:hover {
  transform: translateX(5px);
  box-shadow: 0 8px 25px rgba(102, 126, 234, 0.1);
}

.abstract-section h4 {
  color: #667eea;
  margin-bottom: 1rem;
  font-size: 1.1rem;
  font-weight: 700;
}

.abstract-section p {
  line-height: 1.7;
  color: #444;
  margin: 0;
  font-size: 0.9rem;
}

/* Keywords with Stagger Effect */
.keywords-section {
  display: flex;
  flex-wrap: wrap;
  gap: 0.8rem;
  margin-top: 2rem;
}

.keyword {
  background: linear-gradient(45deg, 
    rgba(102, 126, 234, 0.1), 
    rgba(240, 93, 251, 0.1)
  );
  color: #667eea;
  padding: 0.5rem 1rem;
  border-radius: 25px;
  font-size: 0.8rem;
  font-weight: 500;
  border: 1px solid rgba(102, 126, 234, 0.2);
  transition: all 0.3s ease;
  animation: fadeInUp var(--delay, 2.2s) ease-out;
}

.keyword:nth-child(1) { --delay: 2.2s; }
.keyword:nth-child(2) { --delay: 2.4s; }
.keyword:nth-child(3) { --delay: 2.6s; }
.keyword:nth-child(4) { --delay: 2.8s; }
.keyword:nth-child(5) { --delay: 3.0s; }

.keyword:hover {
  background: linear-gradient(45deg, #667eea, #764ba2);
  color: white;
  transform: translateY(-2px) scale(1.05);
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
}

/* Research Impact Section */
.research-impact {
  background: rgba(255, 255, 255, 0.95);
  padding: 2.5rem;
  border-radius: 16px;
  margin: 3rem 0;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.06);
  animation: fadeInUp 2.5s ease-out;
  transition: all 0.3s ease;
}

.research-impact:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
}

.research-impact h3 {
  color: #2c3e50;
  font-size: 1.3rem;
  margin-bottom: 1.5rem;
  text-align: center;
}

.impact-highlights {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.highlight-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background: linear-gradient(135deg, 
    rgba(102, 126, 234, 0.05), 
    rgba(240, 93, 251, 0.05)
  );
  border-radius: 12px;
  transition: all 0.3s ease;
  animation: slideInLeft var(--delay, 3s) ease-out;
}

.highlight-item:nth-child(1) { --delay: 3s; }
.highlight-item:nth-child(2) { --delay: 3.2s; }
.highlight-item:nth-child(3) { --delay: 3.4s; }

.highlight-item:hover {
  background: linear-gradient(135deg, 
    rgba(102, 126, 234, 0.1), 
    rgba(240, 93, 251, 0.1)
  );
  transform: translateX(5px);
}

.highlight-icon {
  font-size: 2rem;
  min-width: 3rem;
  text-align: center;
}

.highlight-text {
  color: #555;
  font-size: 0.9rem;
  line-height: 1.4;
  font-weight: 500;
}

/* Responsive Design */
@media (max-width: 768px) {
  .publications-wrapper {
    padding: 1.5rem;
    margin: 0 0.5rem;
  }
  
  .publication-card {
    padding: 1.8rem;
  }
  
  .section-title {
    font-size: 1.5rem;
  }
  
  .impact-highlights {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .publication-title {
    font-size: 1.1rem;
  }
  
  .read-paper-btn {
    padding: 0.8rem 1.5rem;
    font-size: 0.85rem;
  }
}
</style>

<div class="publications-wrapper">

<h2 class="section-title">Peer-Reviewed Publications</h2>

<div class="publication-card">
  <span class="year-badge">2024</span>
  
  <h3 class="publication-title">
    <a href="https://chemistry-europe.onlinelibrary.wiley.com/doi/abs/10.1002/slct.202400762" target="_blank">
      Fruit Peel Derived Carbon Dots for Improved Curcumin Delivery: A Promising Strategy for Enhanced Antimicrobial and Antioxidant Activity
    </a>
  </h3>
  
  <div class="authors">
    <strong>Patel, P. J.</strong>, Gupte, S., Naik, R., Kailasa, S. K., Jha, S., Patel, S. B., & Mehta, V. N.
  </div>
  
  <div class="journal-info">
    <em>Chemistry Select</em>, Volume 9, Issue 32, e202400762 (2024) • Impact Factor: 2.3
  </div>
  
  <div style="margin: 1.5rem 0;">
    <a href="https://doi.org/10.1002/slct.202400762" target="_blank" class="read-paper-btn">
      Read Full Paper
    </a>
  </div>
  
  <div class="abstract-section">
    <h4>Abstract</h4>
    <p>Curcumin, known for its proapoptotic, chemo-preventive, chemo-therapeutic, antioxidant, anti-inflammatory, anticancer, and antimicrobial properties, suffers from poor bioavailability, limiting its applications. This study aims to enhance curcumin's bioavailability using carbon dots (CDs) synthesized from fruit peels as a novel nano formulation. CDs were synthesized via hydrothermal synthesis using banana and orange peels as carbon sources. The synthesized CDs were characterized using various techniques including UV-visible spectroscopy, fluorescence spectroscopy, FTIR, DLS, and HRTEM. The results demonstrated successful formation of spherical CDs with enhanced curcumin delivery properties and improved antimicrobial and antioxidant activities.</p>
  </div>
  
  <div class="keywords-section">
    <span class="keyword">Carbon Dots</span>
    <span class="keyword">Curcumin</span>
    <span class="keyword">Drug Delivery</span>
    <span class="keyword">Nanotechnology</span>
    <span class="keyword">Green Synthesis</span>
  </div>
</div>

<div class="research-impact">
  <h3>Research Impact & Significance</h3>
  <p style="color: #555; font-size: 0.95rem; line-height: 1.6; text-align: center; margin-bottom: 2rem;">
    This publication represents a significant contribution to <strong>sustainable nanomedicine</strong>. By utilizing agricultural waste (fruit peels) to create carbon nanodots, this research addresses both environmental sustainability and pharmaceutical efficacy challenges.
  </p>
  
  <div class="impact-highlights">
    <div class="highlight-item">
      <div class="highlight-icon">🌱</div>
      <div class="highlight-text">Green synthesis approach using biodegradable waste materials</div>
    </div>
    <div class="highlight-item">
      <div class="highlight-icon">💊</div>
      <div class="highlight-text">Enhanced bioavailability of curcumin through nanocarrier technology</div>
    </div>
    <div class="highlight-item">
      <div class="highlight-icon">🧪</div>
      <div class="highlight-text">Comprehensive characterization using multiple analytical techniques</div>
    </div>
  </div>
</div>

</div>
