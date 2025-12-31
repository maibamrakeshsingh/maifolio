---
layout: homepage
---

<!-- Profile Section -->
<div class="profile-card">
    <h2><img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/profile-icon.png" alt="Profile" class="section-icon-img"> Personal Statement</h2>
    <div class="profile-content">
        <img src="assets/img/ppp.png" alt="Maibam R. Singh" class="profile-image">
        <div class="statement-text">
            <p>
               <img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/microscope-icon.png" alt="Research" class="inline-icon-img"> I am currently seeking <strong>Ph.D. opportunities in Mathematical Statistics and Mathematical Statistical Physics</strong>, with a strong emphasis on the mathematical foundations of stochastic systems and random processes. My research lies at the intersection of <strong>randomness, geometry, and complex dynamical systems</strong>, where I study how local stochastic interactions give rise to emergent macroscopic behavior.
            </p>
            
            <p>
                My approach combines rigorous mathematical analysis with computational methods to explore phenomena across scales—from microscopic particle interactions to macroscopic phase transitions in complex systems.
            </p>
            
            <h3><img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/interests-icon.png" alt="Interests" class="section-icon-img"> Core Research Interests</h3>
            <ul class="research-interests">
                <li><strong>Complex Systems & Emergent Phenomena</strong></li>
                <li><strong>Probability Theory & Stochastic Processes</strong></li>
                <li><strong>Percolation Theory & Phase Transitions</strong></li>
                <li><strong>Interacting Particle Systems</strong></li>
                <li><strong>Stochastic & Random Geometry</strong></li>
            </ul>
            
            <h3><img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/vision-icon.png" alt="Vision" class="section-icon-img"> Research Vision</h3>
            <p>
                My work bridges discrete and continuous stochastic modeling with applications in <strong>statistical mechanics, percolation theory, random geometry, and interacting particle systems</strong>. I aim to advance the theoretical understanding of <strong>probability, mathematical physics, and statistical geometry</strong> through rigorous mathematical analysis and formulation.
            </p>
            
            <h3><img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/work-icon.png" alt="Work" class="section-icon-img"> Applied & Collaborative Work</h3>
            <p>
                Alongside my academic pursuits, I engage in <strong>Data Science and MLOps projects</strong>, applying statistical modeling and computational techniques to solve real-world problems.
            </p>
        </div>
    </div>
</div>

<!-- Publications Section -->
<div class="publications-card">
    <h2><img src="https://raw.githubusercontent.com/maibamrakeshsingh/maibamrakeshsingh.github.io/main/assets/icons/projects-icon.png" alt="Projects" class="section-icon-img"> Projects & Portfolios</h2>
    {% include_relative _includes/publications.md %}
</div>

<!-- CSS Styles -->
<style>
.profile-card, .publications-card {
    border: 1px solid #e0e0e0;
    border-radius: 12px;
    padding: 30px;
    margin-bottom: 35px;
    background: #ffffff;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.profile-card:hover, .publications-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 16px rgba(0,0,0,0.12);
}

.profile-card h2, .publications-card h2 {
    color: #2c5282;
    border-bottom: 3px solid #2c5282;
    padding-bottom: 12px;
    margin-top: 0;
    margin-bottom: 25px;
    font-weight: 700;
    font-size: 1.8rem;
    display: flex;
    align-items: center;
    gap: 12px;
}

h3 {
    color: #2c5282;
    margin-top: 25px;
    margin-bottom: 15px;
    font-weight: 600;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-icon-img {
    width: 28px;
    height: 28px;
    object-fit: contain;
}

.inline-icon-img {
    width: 20px;
    height: 20px;
    object-fit: contain;
    margin-right: 8px;
    vertical-align: middle;
}

.profile-content {
    display: flex;
    align-items: flex-start;
    gap: 35px;
    margin-top: 15px;
}

.profile-image {
    width: 170px;
    height: 170px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #2c5282;
    box-shadow: 0 5px 15px rgba(44, 82, 130, 0.2);
    flex-shrink: 0;
}

.statement-text {
    flex: 1;
    font-size: 1.08rem;
    line-height: 1.75;
    color: #333;
}

.statement-text p {
    margin-bottom: 20px;
}

.research-interests {
    list-style: none;
    padding-left: 0;
    margin: 15px 0;
}

.research-interests li {
    padding: 8px 0;
    padding-left: 25px;
    position: relative;
    margin-bottom: 5px;
}

.research-interests li:before {
    content: "▸";
    color: #2c5282;
    font-weight: bold;
    position: absolute;
    left: 0;
}

/* Dark Mode Support */
@media (prefers-color-scheme: dark) {
    .profile-card, .publications-card {
        background: #1e1e1e;
        border-color: #404040;
        box-shadow: 0 4px 12px rgba(0,0,0,0.25);
    }
    
    .profile-card h2, .publications-card h2 {
        color: #63b3ed;
        border-bottom-color: #63b3ed;
    }
    
    h3 {
        color: #63b3ed;
    }
    
    .statement-text {
        color: #e2e8f0;
    }
    
    .profile-image {
        border-color: #63b3ed;
        box-shadow: 0 5px 15px rgba(99, 179, 237, 0.25);
    }
    
    .research-interests li:before {
        color: #63b3ed;
    }
    
    /* Invert icon colors for dark mode if needed */
    .section-icon-img, .inline-icon-img {
        filter: invert(1) brightness(1.5);
    }
}

/* Responsive Design */
@media (max-width: 768px) {
    .profile-content {
        flex-direction: column;
        align-items: center;
        text-align: center;
        gap: 25px;
    }
    
    .profile-image {
        width: 150px;
        height: 150px;
    }
    
    .profile-card, .publications-card {
        padding: 20px;
    }
    
    .research-interests li {
        padding-left: 0;
        text-align: left;
    }
    
    .research-interests li:before {
        position: static;
        margin-right: 8px;
    }
    
    .profile-card h2, .publications-card h2, h3 {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
    }
    
    .section-icon-img {
        width: 24px;
        height: 24px;
    }
    
    .inline-icon-img {
        width: 18px;
        height: 18px;
    }
}
</style>
