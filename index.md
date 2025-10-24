---
layout: default
---

<div class="hero-section">
  <div class="hero-content">
    <h1 class="hero-title">Welcome to My Portfolio</h1>
    <p class="hero-subtitle">I'm Subhash Singh, a passionate developer and technology enthusiast</p>
    <div class="hero-buttons">
      <a href="/about/" class="btn btn-primary">Learn More About Me</a>
      <a href="/projects/" class="btn btn-secondary">View My Projects</a>
    </div>
  </div>
</div>

<section class="featured-section">
  <div class="container">
    <h2>Featured Work</h2>
    <div class="featured-grid">
      {% for project in site.projects limit:3 %}
      <div class="featured-item">
        <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
        <p>{{ project.description }}</p>
        <div class="tech-tags">
          {% for tag in project.tech %}
          <span class="tag">{{ tag }}</span>
          {% endfor %}
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<section class="skills-section">
  <div class="container">
    <h2>Technical Skills</h2>
    <div class="skills-grid">
      <div class="skill-category">
        <h3>Languages</h3>
        <ul>
          <li>JavaScript/TypeScript</li>
          <li>Python</li>
          <li>C#/.NET</li>
          <li>Java</li>
        </ul>
      </div>
      <div class="skill-category">
        <h3>Frameworks</h3>
        <ul>
          <li>React/Next.js</li>
          <li>Node.js</li>
          <li>ASP.NET Core</li>
          <li>Spring Boot</li>
        </ul>
      </div>
      <div class="skill-category">
        <h3>Cloud & DevOps</h3>
        <ul>
          <li>Azure</li>
          <li>AWS</li>
          <li>Docker</li>
          <li>Kubernetes</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section class="recent-posts">
  <div class="container">
    <h2>Recent Blog Posts</h2>
    <div class="posts-grid">
      {% for post in site.posts limit:3 %}
      <article class="post-preview">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
        <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      </article>
      {% endfor %}
    </div>
  </div>
</section>

<style>
.hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 100px 0;
  text-align: center;
}

.hero-title {
  font-size: 3.5rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.hero-subtitle {
  font-size: 1.5rem;
  margin-bottom: 2rem;
  opacity: 0.9;
}

.hero-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

.btn {
  padding: 12px 24px;
  text-decoration: none;
  border-radius: 6px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-primary {
  background: white;
  color: #667eea;
}

.btn-secondary {
  background: transparent;
  color: white;
  border: 2px solid white;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

.featured-section, .skills-section, .recent-posts {
  padding: 60px 0;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.featured-grid, .skills-grid, .posts-grid {
  display: grid;
  gap: 2rem;
  margin-top: 2rem;
}

.featured-grid {
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.skills-grid {
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}

.posts-grid {
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}

.featured-item, .skill-category, .post-preview {
  background: #f8f9fa;
  padding: 2rem;
  border-radius: 8px;
  border-left: 4px solid #667eea;
}

.tech-tags {
  margin-top: 1rem;
}

.tag {
  display: inline-block;
  background: #667eea;
  color: white;
  padding: 4px 8px;
  border-radius: 4px;
  font-size: 0.8rem;
  margin-right: 0.5rem;
  margin-bottom: 0.5rem;
}

.skill-category ul {
  list-style: none;
  padding: 0;
}

.skill-category li {
  padding: 0.5rem 0;
  border-bottom: 1px solid #eee;
}

.post-meta {
  color: #666;
  font-size: 0.9rem;
}
</style>