---
layout: homepage
---

<!-- Profile Section with Boundary -->
<div class="section-boundary">
## Profile
<div class="profile-container">
  <img src="assets/img/avatar.png" alt="Maibam R. Singh" class="profile-image">
  <div class="profile-content">
    I am a Ph.D. student at ...
  </div>
</div>
</div>

<!-- Personal Statement Section with Boundary -->
<div class="section-boundary">
## Personal Statement 
I am a Ph.D. student at ...
</div>

<!-- Publications Section with Boundary -->
<div class="section-boundary">
{% include_relative _includes/publications.md %}
</div>

<!-- Services Section with Boundary -->
<div class="section-boundary">
{% include_relative _includes/services.md %}
</div>

<!-- Custom CSS for Boundaries and Image -->
<style>
.section-boundary {
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 20px;
  margin-bottom: 30px;
  background-color: #ffffff;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  transition: box-shadow 0.3s ease;
}

.section-boundary:hover {
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.profile-container {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin-top: 20px;
}

.profile-image {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid #4a6fa5;
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.profile-content {
  flex: 1;
  line-height: 1.6;
  font-size: 1.1em;
}

/* Dark mode support */
@media (prefers-color-scheme: dark) {
  .section-boundary {
    border-color: #404040;
    background-color: #1a1a1a;
    box-shadow: 0 2px 4px rgba(0,0,0,0.2);
  }
  
  .section-boundary:hover {
    box-shadow: 0 4px 8px rgba(0,0,0,0.3);
  }
  
  .profile-image {
    border-color: #2c5282;
  }
}

/* Responsive design */
@media (max-width: 768px) {
  .profile-container {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  
  .profile-image {
    width: 180px;
    height: 180px;
  }
  
  .section-boundary {
    padding: 15px;
    margin-bottom: 20px;
  }
}
</style>
