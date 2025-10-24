---
layout: default
title: Projects
permalink: /projects/
---

# My Projects

<div class="projects-intro">
  <p>Here's a showcase of some of my recent projects. Each project represents a unique challenge and learning opportunity.</p>
</div>

<div class="projects-filter">
  <button class="filter-btn active" data-filter="all">All Projects</button>
  <button class="filter-btn" data-filter="web">Web Development</button>
  <button class="filter-btn" data-filter="ai">AI/ML</button>
  <button class="filter-btn" data-filter="mobile">Mobile</button>
  <button class="filter-btn" data-filter="tools">Tools & Utilities</button>
</div>

<div class="projects-grid">
  <div class="project-card" data-category="web ai">
    <div class="project-image">
      <div class="placeholder-image">AI Web App</div>
    </div>
    <div class="project-content">
      <h3>AI-Powered Task Manager</h3>
      <p>A smart task management application that uses AI to prioritize tasks, suggest deadlines, and provide productivity insights.</p>
      <div class="project-tech">
        <span class="tech-tag">React</span>
        <span class="tech-tag">Python</span>
        <span class="tech-tag">OpenAI API</span>
        <span class="tech-tag">Azure</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">Live Demo</a>
        <a href="#" class="btn btn-sm btn-outline">GitHub</a>
      </div>
    </div>
  </div>

  <div class="project-card" data-category="web">
    <div class="project-image">
      <div class="placeholder-image">E-Commerce</div>
    </div>
    <div class="project-content">
      <h3>Modern E-Commerce Platform</h3>
      <p>A full-stack e-commerce solution with advanced features like real-time inventory, payment processing, and analytics dashboard.</p>
      <div class="project-tech">
        <span class="tech-tag">Next.js</span>
        <span class="tech-tag">Node.js</span>
        <span class="tech-tag">PostgreSQL</span>
        <span class="tech-tag">Stripe</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">Live Demo</a>
        <a href="#" class="btn btn-sm btn-outline">GitHub</a>
      </div>
    </div>
  </div>

  <div class="project-card" data-category="tools">
    <div class="project-image">
      <div class="placeholder-image">DevOps Tool</div>
    </div>
    <div class="project-content">
      <h3>Automated Deployment Pipeline</h3>
      <p>A comprehensive CI/CD pipeline tool that automates testing, building, and deployment processes for multiple environments.</p>
      <div class="project-tech">
        <span class="tech-tag">Docker</span>
        <span class="tech-tag">Kubernetes</span>
        <span class="tech-tag">GitHub Actions</span>
        <span class="tech-tag">Terraform</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">Documentation</a>
        <a href="#" class="btn btn-sm btn-outline">GitHub</a>
      </div>
    </div>
  </div>

  <div class="project-card" data-category="mobile">
    <div class="project-image">
      <div class="placeholder-image">Mobile App</div>
    </div>
    <div class="project-content">
      <h3>Fitness Tracking App</h3>
      <p>A cross-platform mobile app for tracking workouts, nutrition, and health metrics with social features and challenges.</p>
      <div class="project-tech">
        <span class="tech-tag">React Native</span>
        <span class="tech-tag">Firebase</span>
        <span class="tech-tag">Redux</span>
        <span class="tech-tag">Health APIs</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">App Store</a>
        <a href="#" class="btn btn-sm btn-outline">GitHub</a>
      </div>
    </div>
  </div>

  <div class="project-card" data-category="ai">
    <div class="project-image">
      <div class="placeholder-image">ML Model</div>
    </div>
    <div class="project-content">
      <h3>Predictive Analytics Dashboard</h3>
      <p>Machine learning model for predicting customer behavior and sales trends with an interactive dashboard for business insights.</p>
      <div class="project-tech">
        <span class="tech-tag">Python</span>
        <span class="tech-tag">TensorFlow</span>
        <span class="tech-tag">Pandas</span>
        <span class="tech-tag">Streamlit</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">Live Demo</a>
        <a href="#" class="btn btn-sm btn-outline">GitHub</a>
      </div>
    </div>
  </div>

  <div class="project-card" data-category="web tools">
    <div class="project-image">
      <div class="placeholder-image">API Tool</div>
    </div>
    <div class="project-content">
      <h3>API Development Framework</h3>
      <p>A lightweight framework for rapidly building RESTful APIs with built-in authentication, validation, and documentation.</p>
      <div class="project-tech">
        <span class="tech-tag">Node.js</span>
        <span class="tech-tag">Express</span>
        <span class="tech-tag">JWT</span>
        <span class="tech-tag">Swagger</span>
      </div>
      <div class="project-links">
        <a href="#" class="btn btn-sm">Documentation</a>
        <a href="#" class="btn btn-sm btn-outline">NPM</a>
      </div>
    </div>
  </div>
</div>

<div class="cta-section">
  <h2>Interested in Working Together?</h2>
  <p>I'm always open to discussing new projects and opportunities.</p>
  <a href="/contact/" class="btn btn-primary btn-lg">Let's Talk</a>
</div>

<style>
.projects-intro {
  text-align: center;
  margin: 2rem 0;
}

.projects-intro p {
  font-size: 1.2rem;
  color: #666;
  max-width: 600px;
  margin: 0 auto;
}

.projects-filter {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin: 3rem 0;
  flex-wrap: wrap;
}

.filter-btn {
  padding: 8px 16px;
  border: 2px solid #667eea;
  background: white;
  color: #667eea;
  border-radius: 25px;
  cursor: pointer;
  transition: all 0.3s ease;
  font-weight: 500;
}

.filter-btn:hover,
.filter-btn.active {
  background: #667eea;
  color: white;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.project-card {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
  border: 1px solid #e1e8ed;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

.project-image {
  height: 200px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  display: flex;
  align-items: center;
  justify-content: center;
}

.placeholder-image {
  color: white;
  font-size: 1.5rem;
  font-weight: 600;
}

.project-content {
  padding: 2rem;
}

.project-content h3 {
  margin-bottom: 1rem;
  color: #333;
}

.project-content p {
  color: #666;
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.project-tech {
  margin-bottom: 1.5rem;
}

.tech-tag {
  display: inline-block;
  background: #f1f3f4;
  color: #333;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 0.8rem;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
}

.project-links {
  display: flex;
  gap: 1rem;
}

.btn {
  padding: 8px 16px;
  text-decoration: none;
  border-radius: 6px;
  font-weight: 500;
  transition: all 0.3s ease;
  border: none;
  cursor: pointer;
  display: inline-block;
  text-align: center;
}

.btn-sm {
  padding: 6px 12px;
  font-size: 0.9rem;
}

.btn-lg {
  padding: 16px 32px;
  font-size: 1.1rem;
}

.btn-primary {
  background: #667eea;
  color: white;
}

.btn-outline {
  background: transparent;
  color: #667eea;
  border: 1px solid #667eea;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
}

.cta-section {
  text-align: center;
  padding: 4rem 2rem;
  background: #f8f9fa;
  border-radius: 12px;
  margin-top: 4rem;
}

.cta-section h2 {
  margin-bottom: 1rem;
  color: #333;
}

.cta-section p {
  color: #666;
  font-size: 1.1rem;
  margin-bottom: 2rem;
}

@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
  }
  
  .projects-filter {
    flex-direction: column;
    align-items: center;
  }
  
  .project-links {
    flex-direction: column;
  }
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const filterBtns = document.querySelectorAll('.filter-btn');
  const projectCards = document.querySelectorAll('.project-card');
  
  filterBtns.forEach(btn => {
    btn.addEventListener('click', function() {
      // Remove active class from all buttons
      filterBtns.forEach(b => b.classList.remove('active'));
      // Add active class to clicked button
      this.classList.add('active');
      
      const filter = this.getAttribute('data-filter');
      
      projectCards.forEach(card => {
        if (filter === 'all') {
          card.style.display = 'block';
        } else {
          const categories = card.getAttribute('data-category').split(' ');
          if (categories.includes(filter)) {
            card.style.display = 'block';
          } else {
            card.style.display = 'none';
          }
        }
      });
    });
  });
});
</script>