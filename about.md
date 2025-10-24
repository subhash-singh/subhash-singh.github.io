---
layout: default
title: About
permalink: /about/
---

# About Me

<div class="about-container">
  <div class="about-text">
    <p class="lead">Hello! I'm Subhash Singh, a passionate software developer with expertise in building scalable applications and innovative solutions.</p>
    
    <p>With several years of experience in the technology industry, I specialize in:</p>
    
    <ul class="expertise-list">
      <li><strong>Full-Stack Development:</strong> Building end-to-end applications using modern frameworks</li>
      <li><strong>Cloud Architecture:</strong> Designing and implementing cloud-native solutions</li>
      <li><strong>AI & Machine Learning:</strong> Developing intelligent applications and automation</li>
      <li><strong>DevOps & CI/CD:</strong> Streamlining development and deployment processes</li>
    </ul>
    
    <h2>My Journey</h2>
    <p>My journey in technology started with a curiosity about how things work. This curiosity led me to explore various programming languages, frameworks, and technologies. I believe in continuous learning and staying updated with the latest trends in technology.</p>
    
    <h2>What I Do</h2>
    <p>Currently, I work on various projects ranging from web applications to AI-powered solutions. I enjoy solving complex problems and creating user-friendly applications that make a difference.</p>
    
    <h2>Beyond Code</h2>
    <p>When I'm not coding, you can find me:</p>
    <ul>
      <li>Reading about emerging technologies</li>
      <li>Contributing to open-source projects</li>
      <li>Writing technical articles and tutorials</li>
      <li>Mentoring aspiring developers</li>
    </ul>
    
    <div class="contact-cta">
      <h3>Let's Connect!</h3>
      <p>I'm always interested in discussing new opportunities, collaborations, or just chatting about technology.</p>
      <a href="/contact/" class="btn btn-primary">Get In Touch</a>
    </div>
  </div>
  
  <div class="about-sidebar">
    <div class="stats-card">
      <h3>Quick Stats</h3>
      <div class="stat-item">
        <span class="stat-number">5+</span>
        <span class="stat-label">Years Experience</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">50+</span>
        <span class="stat-label">Projects Completed</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">10+</span>
        <span class="stat-label">Technologies</span>
      </div>
    </div>
    
    <div class="tech-stack">
      <h3>Current Tech Stack</h3>
      <div class="tech-categories">
        <div class="tech-category">
          <h4>Frontend</h4>
          <span class="tech-tag">React</span>
          <span class="tech-tag">TypeScript</span>
          <span class="tech-tag">Next.js</span>
          <span class="tech-tag">Tailwind CSS</span>
        </div>
        <div class="tech-category">
          <h4>Backend</h4>
          <span class="tech-tag">Node.js</span>
          <span class="tech-tag">.NET Core</span>
          <span class="tech-tag">Python</span>
          <span class="tech-tag">PostgreSQL</span>
        </div>
        <div class="tech-category">
          <h4>Cloud & DevOps</h4>
          <span class="tech-tag">Azure</span>
          <span class="tech-tag">Docker</span>
          <span class="tech-tag">GitHub Actions</span>
          <span class="tech-tag">Terraform</span>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
.about-container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 3rem;
  margin-top: 2rem;
}

.lead {
  font-size: 1.25rem;
  color: #555;
  margin-bottom: 2rem;
}

.expertise-list {
  margin: 2rem 0;
}

.expertise-list li {
  margin-bottom: 1rem;
  padding-left: 1rem;
}

.about-sidebar {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.stats-card, .tech-stack {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 8px;
  border-left: 4px solid #667eea;
}

.stat-item {
  display: flex;
  flex-direction: column;
  text-align: center;
  margin-bottom: 1.5rem;
}

.stat-number {
  font-size: 2.5rem;
  font-weight: 700;
  color: #667eea;
}

.stat-label {
  font-size: 0.9rem;
  color: #666;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.tech-categories {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.tech-category h4 {
  margin-bottom: 0.5rem;
  color: #333;
}

.tech-tag {
  display: inline-block;
  background: #667eea;
  color: white;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 0.8rem;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
}

.contact-cta {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 2rem;
  border-radius: 8px;
  text-align: center;
  margin-top: 3rem;
}

.contact-cta .btn {
  background: white;
  color: #667eea;
  padding: 12px 24px;
  text-decoration: none;
  border-radius: 6px;
  font-weight: 600;
  display: inline-block;
  margin-top: 1rem;
  transition: all 0.3s ease;
}

.contact-cta .btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

@media (max-width: 768px) {
  .about-container {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
}
</style>