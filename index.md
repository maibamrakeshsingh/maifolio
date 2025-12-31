---
layout: homepage
---

<!-- Profile Section -->
<div style="border: 1px solid #e0e0e0; border-radius: 10px; padding: 25px; margin-bottom: 30px; background: #ffffff; box-shadow: 0 2px 8px rgba(0,0,0,0.05);">
<h2 style="color: #2c5282; border-bottom: 2px solid #2c5282; padding-bottom: 10px; margin-top: 0; margin-bottom: 20px; font-weight: 600;">Personal Statement</h2>
<div style="display: flex; align-items: flex-start; gap: 30px; margin-top: 15px;">
  <img src="assets/img/ppp.png" alt="Maibam R. Singh" style="width: 160px; height: 160px; border-radius: 50%; object-fit: cover; border: 3px solid #2c5282; box-shadow: 0 4px 12px rgba(44, 82, 130, 0.15);">
  <div style="flex: 1; font-size: 1.05em; line-height: 1.7; color: #333;">
    I am currently seeking **Ph.D. opportunities in Mathematical Statistics and Mathematical Statistical Physics**, with a strong emphasis on the mathematical foundations of stochastic systems and random processes. My research lies at the intersection of **randomness, geometry, and complex dynamical systems**, where I study how local stochastic interactions give rise to emergent macroscopic behavior.

📌 **Core Research Interests**  
- **Complex Systems & Emergent Phenomena**  
- **Probability Theory & Stochastic Processes**  
- **Percolation Theory & Phase Transitions**  
- **Interacting Particle Systems**  
- **Stochastic & Random Geometry**

🎯 **Research Vision**  
My work bridges discrete and continuous stochastic modeling with applications in **statistical mechanics, percolation theory, random geometry, and interacting particle systems**. I aim to advance the theoretical understanding of **probability, mathematical physics, and statistical geometry** through rigorous mathematical analysis and formulation.

💼 **Applied & Collaborative Work**  
Alongside my academic pursuits, I engage in **Data Science and MLOps projects**, applying statistical modeling and computational techniques to solve real-world problems.
  </div>
</div>
</div>

<!-- Publications Section -->
<div style="border: 1px solid #e0e0e0; border-radius: 10px; padding: 25px; margin-bottom: 30px; background: #ffffff; box-shadow: 0 2px 8px rgba(0,0,0,0.05);">
<h2 style="color: #2c5282; border-bottom: 2px solid #2c5282; padding-bottom: 10px; margin-top: 0; margin-bottom: 20px; font-weight: 600;">Projects & Portfolios</h2>
{% include_relative _includes/publications.md %}
</div>

<!-- Dark Mode Support -->
<style>
@media (prefers-color-scheme: dark) {
  div[style*="background: #ffffff"] {
    background: #1a1a1a !important;
    border-color: #404040 !important;
  }
  
  h2[style*="color: #2c5282"] {
    color: #63b3ed !important;
    border-bottom-color: #63b3ed !important;
  }
  
  div[style*="color: #333"] {
    color: #e2e8f0 !important;
  }
  
  img[style*="border: 3px solid #2c5282"] {
    border-color: #63b3ed !important;
    box-shadow: 0 4px 12px rgba(99, 179, 237, 0.2) !important;
  }
}
</style>
