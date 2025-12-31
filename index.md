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
        <img src="assets/img/ppp.png" alt="Maibam R. Singh" class="profile-image">
        <div class="statement-text">
            <p>
               🔬 I am currently seeking <strong>Ph.D. opportunities in Mathematical Statistics and Mathematical Statistical Physics</strong>, with a strong emphasis on the mathematical foundations of stochastic systems and random processes. My research lies at the intersection of <strong>randomness, geometry, and complex dynamical systems</strong>, where I study how local stochastic interactions give rise to emergent macroscopic behavior.
            </p>
            
            <p>
                My approach combines rigorous mathematical analysis with computational methods to explore phenomena across scales—from microscopic particle interactions to macroscopic phase transitions in complex systems.
            </p>
            
            <h3>📌 Core Research Interests</h3>
            <ul class="research-interests">
                <li><strong>Complex Systems & Emergent Phenomena</strong></li>
                <li><strong>Probability Theory & Stochastic Processes</strong></li>
                <li><strong>Percolation Theory & Phase Transitions</strong></li>
                <li><strong>Interacting Particle Systems</strong></li>
                <li><strong>Stochastic & Random Geometry</strong></li>
            </ul>
            
            <h3>🎯 Research Vision</h3>
            <p>
                My work bridges discrete and continuous stochastic modeling with applications in <strong>statistical mechanics, percolation theory, random geometry, and interacting particle systems</strong>. I aim to advance the theoretical understanding of <strong>probability, mathematical physics, and statistical geometry</strong> through rigorous mathematical analysis and formulation.
            </p>
            
            <h3>💼 Applied & Collaborative Work</h3>
            <p>
                Alongside my academic pursuits, I engage in <strong>Data Science and MLOps projects</strong>, applying statistical modeling and computational techniques to solve real-world problems.
            </p>
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
.profile-card, .publications-card {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 30px;
    margin-bottom: 30px;
    background: white;
    transition: all 0.3s ease;
    box-shadow: 0 3px 10px rgba(0,0,0,0.08);
    overflow: hidden;
}

.profile-card:hover, .publications-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 16px rgba(0,0,0,0.12);
}

.section-header {
    margin-bottom: 25px;
    position: relative;
}

.profile-card h2, .publications-card h2 {
    color: #2c5282;
    padding-bottom: 8px;
    margin-top: 0;
    margin-bottom: 0;
    font-weight: 700;
    font-size: 1.8rem;
    display: inline-block;
}

.title-underline {
    height: 3px;
    width: 100%;
    background: #2c5282;
    margin-top: 5px;
    border-radius: 2px;
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
    align-self: flex-start;
}

.statement-text {
    flex: 1;
    font-size: 1.08rem;
    line-height: 1.75;
    color: #333;
}

.statement-text p {
    margin-bottom: 20px;
    text-align: justify;
}

.statement-text h3 {
    color: #2c5282;
    margin-top: 25px;
    margin-bottom: 15px;
    font-weight: 600;
    font-size: 1.3rem;
}

.research-interests {
    list-style: none;
    padding-left: 0;
    margin: 15px 0;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 8px;
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
    }
    
    .title-underline {
        background: #63b3ed;
    }
    
    .statement-text {
        color: #e2e8f0;
    }
    
    .statement-text h3 {
        color: #63b3ed;
    }
    
    .profile-image {
        border-color: #63b3ed;
        box-shadow: 0 5px 15px rgba(99, 179, 237, 0.25);
    }
    
    .research-interests li:before {
        color: #63b3ed;
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
        align-self: center;
    }
    
    .statement-text {
        text-align: left;
    }
    
    .profile-card, .publications-card {
        padding: 20px;
    }
    
    .research-interests {
        grid-template-columns: 1fr;
    }
    
    .research-interests li {
        padding-left: 0;
        text-align: left;
    }
    
    .research-interests li:before {
        position: static;
        margin-right: 8px;
    }
    
    .statement-text h3 {
        text-align: left;
    }
}

@media (max-width: 480px) {
    .profile-card, .publications-card {
        padding: 15px;
    }
    
    .profile-card h2, .publications-card h2 {
        font-size: 1.5rem;
    }
    
    .statement-text {
        font-size: 1rem;
    }
}
</style>
