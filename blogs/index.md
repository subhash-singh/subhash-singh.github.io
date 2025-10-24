---
layout: default
title: Blog
permalink: /blog/
---

# Blog

<div class="blog-intro">
  <p>Welcome to my blog! Here I share insights, tutorials, and thoughts about technology, development, and innovation.</p>
</div>

<div class="blog-container">
  <div class="blog-posts">
    {% for post in site.posts %}
    <article class="blog-post-card">
      <div class="post-header">
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <div class="post-meta">
          <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
          {% if post.categories %}
          <span class="post-categories">
            {% for category in post.categories %}
            <span class="category-tag">{{ category }}</span>
            {% endfor %}
          </span>
          {% endif %}
        </div>
      </div>
      
      <div class="post-excerpt">
        {% if post.excerpt %}
          {{ post.excerpt | strip_html | truncatewords: 50 }}
        {% else %}
          {{ post.content | strip_html | truncatewords: 50 }}
        {% endif %}
      </div>
      
      <div class="post-footer">
        <a href="{{ post.url }}" class="read-more">Read More →</a>
      </div>
    </article>
    {% endfor %}
    
    {% if site.posts.size == 0 %}
    <div class="no-posts">
      <h3>No posts yet!</h3>
      <p>Stay tuned for upcoming content. I'll be sharing insights about technology, development, and more.</p>
    </div>
    {% endif %}
  </div>
  
  <aside class="blog-sidebar">
    <div class="sidebar-section">
      <h3>Categories</h3>
      <div class="categories-list">
        {% assign categories = site.categories | sort %}
        {% for category in categories %}
        <a href="#" class="category-link">
          {{ category[0] }}
          <span class="category-count">({{ category[1].size }})</span>
        </a>
        {% endfor %}
      </div>
    </div>
    
    <div class="sidebar-section">
      <h3>Recent Posts</h3>
      <div class="recent-posts-list">
        {% for post in site.posts limit:5 %}
        <div class="recent-post-item">
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="recent-post-date">{{ post.date | date: "%b %d" }}</span>
        </div>
        {% endfor %}
      </div>
    </div>
    
    <div class="sidebar-section">
      <h3>Archive</h3>
      <div class="archive-list">
        {% assign postsByYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
        {% for year in postsByYear %}
        <div class="archive-year">
          <h4>{{ year.name }}</h4>
          {% assign postsByMonth = year.items | group_by_exp: 'post', 'post.date | date: "%B"' %}
          {% for month in postsByMonth %}
          <div class="archive-month">
            <a href="#">{{ month.name }} ({{ month.items.size }})</a>
          </div>
          {% endfor %}
        </div>
        {% endfor %}
      </div>
    </div>
    
    <div class="sidebar-section">
      <h3>Subscribe</h3>
      <p>Stay updated with new posts and insights.</p>
      <a href="{{ '/feed.xml' | relative_url }}" class="btn btn-outline btn-sm">RSS Feed</a>
    </div>
  </aside>
</div>

<style>
.blog-intro {
  text-align: center;
  margin: 2rem 0 3rem 0;
  padding: 2rem;
  background: #f8f9fa;
  border-radius: 8px;
}

.blog-intro p {
  font-size: 1.2rem;
  color: #666;
  max-width: 600px;
  margin: 0 auto;
}

.blog-container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 3rem;
  margin: 2rem 0;
}

.blog-posts {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.blog-post-card {
  background: white;
  border: 1px solid #e1e8ed;
  border-radius: 12px;
  padding: 2rem;
  transition: all 0.3s ease;
}

.blog-post-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
}

.post-header h2 {
  margin-bottom: 1rem;
}

.post-header h2 a {
  color: #333;
  text-decoration: none;
  transition: color 0.3s ease;
}

.post-header h2 a:hover {
  color: #667eea;
}

.post-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  align-items: center;
  margin-bottom: 1rem;
  font-size: 0.9rem;
  color: #666;
}

.post-date {
  font-weight: 500;
}

.post-categories {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.category-tag {
  background: #667eea;
  color: white;
  padding: 2px 8px;
  border-radius: 12px;
  font-size: 0.8rem;
}

.post-excerpt {
  color: #4a4a4a;
  line-height: 1.6;
  margin-bottom: 1.5rem;
}

.post-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.read-more {
  color: #667eea;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.3s ease;
}

.read-more:hover {
  color: #5a67d8;
  text-decoration: underline;
}

.no-posts {
  text-align: center;
  padding: 4rem 2rem;
  background: #f8f9fa;
  border-radius: 8px;
  color: #666;
}

.blog-sidebar {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.sidebar-section {
  background: #f8f9fa;
  padding: 1.5rem;
  border-radius: 8px;
  border-left: 4px solid #667eea;
}

.sidebar-section h3 {
  margin-bottom: 1rem;
  color: #333;
  font-size: 1.1rem;
}

.categories-list {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.category-link {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0.5rem;
  background: white;
  border-radius: 4px;
  text-decoration: none;
  color: #333;
  transition: all 0.3s ease;
}

.category-link:hover {
  background: #667eea;
  color: white;
  text-decoration: none;
}

.category-count {
  font-size: 0.8rem;
  color: #666;
}

.category-link:hover .category-count {
  color: rgba(255, 255, 255, 0.8);
}

.recent-posts-list {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.recent-post-item {
  display: flex;
  flex-direction: column;
  gap: 0.25rem;
}

.recent-post-item a {
  color: #333;
  text-decoration: none;
  font-weight: 500;
  line-height: 1.3;
}

.recent-post-item a:hover {
  color: #667eea;
  text-decoration: underline;
}

.recent-post-date {
  font-size: 0.8rem;
  color: #666;
}

.archive-list {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.archive-year h4 {
  margin-bottom: 0.5rem;
  color: #333;
  font-size: 1rem;
}

.archive-month {
  margin-left: 1rem;
  margin-bottom: 0.25rem;
}

.archive-month a {
  color: #666;
  text-decoration: none;
  font-size: 0.9rem;
}

.archive-month a:hover {
  color: #667eea;
  text-decoration: underline;
}

@media (max-width: 768px) {
  .blog-container {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
  
  .blog-post-card {
    padding: 1.5rem;
  }
  
  .post-meta {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
  
  .sidebar-section {
    padding: 1rem;
  }
}
</style>