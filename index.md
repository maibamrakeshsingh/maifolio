---
layout: homepage
---

<!-- Profile Section -->
<div class="profile-card">
    <div class="section-header">
        <h2>Personal Statement</h2>
        <div class="title-underline"></div>
    </div>
    
    <div class="profile-content">
        <!-- Main Profile Section -->
        <div class="profile-section">
            <div class="section-content">
                <div class="section-image">
                    <img src="/assets/img/ppp.png" alt="Researcher profile photo">
                </div>
                <div class="section-text">
                    <p>
                       🔬 I am currently seeking <strong>Ph.D. opportunities in Mathematical Statistics and Mathematical Statistical Physics</strong>, with a strong emphasis on the mathematical foundations of stochastic systems and random processes. My research lies at the intersection of <strong>randomness, geometry, and complex dynamical systems</strong>, where I study how local stochastic interactions give rise to emergent macroscopic behavior.
                    </p>
                    <p>
                        My approach combines rigorous mathematical analysis with computational methods to explore phenomena across scales, from microscopic particle interactions to macroscopic phase transitions in complex systems.
                    </p>
                </div>
            </div>
        </div>
        
        <!-- Core Research Interests -->
        <div class="profile-section">
            <div class="section-content">
                <div class="section-image">
                    <img src="/assets/img/research-interests.jpg" alt="Complex systems and network visualization">
                </div>
                <div class="section-text">
                    <h3>📌 Core Research Interests</h3>
                    <ul class="research-interests">
                        <li><strong>Complex Systems & Emergent Phenomena</strong></li>
                        <li><strong>Probability Theory & Stochastic Processes</strong></li>
                        <li><strong>Percolation Theory & Phase Transitions</strong></li>
                        <li><strong>Interacting Particle Systems</strong></li>
                        <li><strong>Stochastic & Random Geometry</strong></li>
                    </ul>
                </div>
            </div>
        </div>
        
        <!-- Research Vision -->
        <div class="profile-section">
            <div class="section-content">
                <div class="section-image">
                    <img src="/assets/img/research-vision.jpg" alt="Research vision and future directions">
                </div>
                <div class="section-text">
                    <h3>🎯 Research Vision</h3>
                    <p>
                        My work bridges discrete and continuous stochastic modeling with applications in <strong>statistical mechanics, percolation theory, random geometry, and interacting particle systems</strong>. I aim to advance the theoretical understanding of <strong>probability, mathematical physics, and statistical geometry</strong> through rigorous mathematical analysis and formulation.
                    </p>
                </div>
            </div>
        </div>
        
        <!-- Applied Work -->
        <div class="profile-section">
            <div class="section-content">
                <div class="section-image">
                    <img src="/assets/img/applied-work.jpg" alt="Data science and machine learning applications">
                </div>
                <div class="section-text">
                    <h3>💼 Applied & Collaborative Work</h3>
                    <p>
                        Alongside my academic pursuits, I engage in <strong>Data Science and MLOps projects</strong>, applying statistical modeling and computational techniques to solve real-world problems.
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>

<!-- Publications Section -->
<div class="publications-card">
    <div class="section-header">
        <h2>Projects & Portfolios</h2>
        <div class="title-underline"></div>
    </div>
    {% include_relative _includes/publications.md %}
</div>

<!-- CSS Styles -->
<style>
/* Base Styles */
.profile-card, .publications-card {
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 35px;
    margin-bottom: 40px;
    background: white;
    transition: all 0.3s ease;
    box-shadow: 0 4px 12px rgba(0,0,0,0.06);
    overflow: hidden;
}

.profile-card:hover, .publications-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.12);
}

.section-header {
    margin-bottom: 35px;
    position: relative;
}

.profile-card h2, .publications-card h2 {
    color: #1a365d;
    padding-bottom: 12px;
    margin-top: 0;
    margin-bottom: 0;
    font-weight: 800;
    font-size: 2.2rem;
    display: inline-block;
    position: relative;
}

.title-underline {
    height: 4px;
    width: 100%;
    background: linear-gradient(90deg, #2c5282, #4299e1);
    margin-top: 8px;
    border-radius: 2px;
}

/* Profile Content Layout */
.profile-content {
    display: flex;
    flex-direction: column;
    gap: 40px;
}

.profile-section {
    padding-bottom: 35px;
    border-bottom: 1px solid #eaeaea;
    transition: all 0.3s ease;
}

.profile-section:hover {
    border-bottom-color: #cbd5e0;
}

.profile-section:last-child {
    padding-bottom: 0;
    border-bottom: none;
}

/* Section Content */
.section-content {
    display: flex;
    align-items: flex-start;
    gap: 30px;
    margin-top: 15px;
}

/* Section Images */
.section-image {
    flex-shrink: 0;
    width: 140px;
    height: 140px;
    border-radius: 50%;
    overflow: hidden;
    border: 4px solid #2c5282;
    box-shadow: 0 6px 20px rgba(44, 82, 130, 0.15);
    transition: all 0.3s ease;
    position: relative;
}

.section-image:hover {
    transform: scale(1.05);
    border-color: #4299e1;
    box-shadow: 0 8px 25px rgba(44, 82, 130, 0.25);
}

.section-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
}

.section-image:hover img {
    transform: scale(1.1);
}

/* Section Text */
.section-text {
    flex: 1;
    min-width: 0; /* Prevent flex item overflow */
}

.section-text h3 {
    color: #2c5282;
    margin-top: 0;
    margin-bottom: 20px;
    font-weight: 700;
    font-size: 1.5rem;
    display: flex;
    align-items: center;
    gap: 12px;
    padding-bottom: 10px;
    border-bottom: 2px solid #e2e8f0;
}

.section-text h3::before {
    font-size: 1.8rem;
}

.section-text p {
    font-size: 1.1rem;
    line-height: 1.8;
    color: #2d3748;
    margin-bottom: 0;
    text-align: justify;
    hyphens: auto;
}

.section-text p + p {
    margin-top: 20px;
}

/* Research Interests */
.research-interests {
    list-style: none;
    padding-left: 0;
    margin: 20px 0;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 15px;
}

.research-interests li {
    padding: 16px 20px;
    padding-left: 45px;
    position: relative;
    background: linear-gradient(135deg, #f7fafc, #edf2f7);
    border-radius: 10px;
    border-left: 5px solid #2c5282;
    transition: all 0.3s ease;
    cursor: default;
}

.research-interests li:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 15px rgba(0,0,0,0.1);
    background: linear-gradient(135deg, #e6fffa, #b2f5ea);
    border-left-color: #38b2ac;
}

.research-interests li:before {
    content: "➤";
    color: #2c5282;
    font-weight: bold;
    font-size: 1.2rem;
    position: absolute;
    left: 18px;
    top: 50%;
    transform: translateY(-50%);
    transition: color 0.3s ease;
}

.research-interests li:hover:before {
    color: #38b2ac;
}

/* Dark Mode Support */
@media (prefers-color-scheme: dark) {
    .profile-card, .publications-card {
        background: #1a202c;
        border-color: #4a5568;
        box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    
    .profile-section {
        border-bottom-color: #4a5568;
    }
    
    .profile-section:hover {
        border-bottom-color: #718096;
    }
    
    .profile-card h2, .publications-card h2 {
        color: #90cdf4;
    }
    
    .title-underline {
        background: linear-gradient(90deg, #63b3ed, #4299e1);
    }
    
    .section-text p {
        color: #e2e8f0;
    }
    
    .section-text h3 {
        color: #90cdf4;
        border-bottom-color: #4a5568;
    }
    
    .section-image {
        border-color: #63b3ed;
        box-shadow: 0 6px 20px rgba(99, 179, 237, 0.2);
    }
    
    .section-image:hover {
        border-color: #90cdf4;
        box-shadow: 0 8px 25px rgba(99, 179, 237, 0.3);
    }
    
    .research-interests li {
        background: linear-gradient(135deg, #2d3748, #4a5568);
        border-left-color: #63b3ed;
    }
    
    .research-interests li:hover {
        background: linear-gradient(135deg, #2c7a7b, #285e61);
        border-left-color: #38b2ac;
    }
    
    .research-interests li:before {
        color: #63b3ed;
    }
    
    .research-interests li:hover:before {
        color: #38b2ac;
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .section-content {
        flex-direction: column;
        align-items: center;
        gap: 25px;
        text-align: center;
    }
    
    .section-image {
        width: 120px;
        height: 120px;
        align-self: center;
    }
    
    .section-text h3 {
        font-size: 1.4rem;
        justify-content: center;
        text-align: center;
    }
    
    .profile-card, .publications-card {
        padding: 25px;
    }
    
    .profile-card h2, .publications-card h2 {
        font-size: 1.8rem;
    }
    
    .profile-content {
        gap: 30px;
    }
    
    .profile-section {
        padding-bottom: 30px;
    }
    
    .research-interests {
        grid-template-columns: 1fr;
        gap: 12px;
    }
    
    .research-interests li {
        padding: 14px 18px;
        padding-left: 40px;
        text-align: left;
    }
    
    .research-interests li:before {
        left: 15px;
    }
    
    .section-text p {
        text-align: left;
    }
}

@media (max-width: 480px) {
    .profile-card, .publications-card {
        padding: 20px;
        margin-bottom: 30px;
    }
    
    .profile-card h2, .publications-card h2 {
        font-size: 1.6rem;
        padding-bottom: 8px;
    }
    
    .section-text p {
        font-size: 1.05rem;
        line-height: 1.7;
    }
    
    .section-image {
        width: 100px;
        height: 100px;
        border-width: 3px;
    }
    
    .section-text h3 {
        font-size: 1.3rem;
        margin-bottom: 15px;
    }
    
    .research-interests li {
        padding: 12px 15px;
        padding-left: 35px;
    }
    
    .research-interests li:before {
        left: 12px;
        font-size: 1.1rem;
    }
}

/* Accessibility improvements */
.section-image img {
    display: block;
}

.section-text strong {
    font-weight: 700;
    color: #2c5282;
}

@media (prefers-color-scheme: dark) {
    .section-text strong {
        color: #90cdf4;
    }
}

/* Smooth scrolling for anchor links */
html {
    scroll-behavior: smooth;
}

/* Focus styles for accessibility */
.section-image:focus,
.research-interests li:focus {
    outline: 3px solid #4299e1;
    outline-offset: 2px;
}

/* Print styles */
@media print {
    .profile-card, .publications-card {
        box-shadow: none;
        border: 1px solid #ccc;
        break-inside: avoid;
    }
    
    .section-image {
        border: 2px solid #333;
        box-shadow: none;
    }
    
    .profile-card:hover, .publications-card:hover {
        transform: none;
        box-shadow: none;
    }
}
</style>
