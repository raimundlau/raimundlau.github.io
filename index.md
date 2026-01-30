---
layout: default
---

<div class="hero-personal">
  <div class="container">
    <div class="hero-content">
      <div class="hero-info-wrapper">
        <div class="hero-text">
           <h1 class="hero-name">{{ site.author | default: "Your Name" }}</h1>
           <p class="hero-title">Robotics & Artificial Intelligence</p>
        </div>
        
        <div class="hero-actions">
          <a href="{{ '/cv.pdf' | relative_url }}" target="_blank" rel="noopener noreferrer" class="btn-secondary">
            CV
          </a>
           <a href="mailto:{{ site.email }}" class="btn-secondary">
            Contact
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="about-section" style="padding: 100px 0; background: var(--surface-color); border-bottom: 1px solid var(--border-color); text-align: center;">
    <div class="container">
        <h1 style="font-size: var(--font-size-3xl); letter-spacing: -0.02em; color: var(--text-primary);">ABOUT ME</h1>
        <p style="color: var(--text-primary); opacity: 0.7; max-width: 600px; margin: 0 auto; font-weight: var(--font-weight-normal);">I am a master student at the Technical University of Munich (TUM) in the field Robotics and AI. I studied Electrical Engineering in my dual bachelor study with the cooperation partner Mercedes-Benz and worked there afterwards for two years before starting the master program.</p>
        <p style="color: var(--text-primary); opacity: 0.7; max-width: 600px; margin: 0 auto; font-weight: var(--font-weight-normal);"></p>
    </div>
</div>


<div class="projects-showcase">
  <div class="container">
    <div class="section-header">
      <h2>Portfolio</h2>
      <p class="section-subtitle">A curated collection of projects</p>
    </div>
    
    <div class="projects-grid-featured">
      {% assign featured_projects = site.projects | where: "featured", true | sort: "date" | reverse %}
      {% assign all_projects = site.projects | sort: "date" | reverse %}
      {% assign combined_projects = featured_projects | concat: all_projects %}
      {% assign unique_projects = combined_projects | uniq %}
      {% for project in unique_projects limit: 3 %}
        <div class="project-card-featured">
          <div class="project-media">
            {% if project.featured_image %}
              <img src="{{ project.featured_image | relative_url }}" alt="{{ project.title }}" class="project-image">
            {% elsif project.models.first %}
              <div class="model-preview-small">
                <model-viewer 
                  src="{{ project.models.first.file | relative_url }}"
                  alt="{{ project.title }}"
                  camera-controls
                  auto-rotate
                  class="preview-model-small">
                </model-viewer>
              </div>
            {% else %}
              <div class="project-placeholder-small">
                <i class="fas fa-robot"></i>
              </div>
            {% endif %}
            
            <div class="project-overlay">
              <a href="{{ project.url | relative_url }}" class="project-link-overlay">
                <i class="fas fa-arrow-right"></i>
              </a>
            </div>
          </div>
          
          <div class="project-info-featured">
            <div class="project-categories-small">
              {% for category in project.categories limit:2 %}
                <span class="category-tag-small">{{ category }}</span>
              {% endfor %}
            </div>
            
            <h3 class="project-title-featured">
              <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
            </h3>
            
            <p class="project-excerpt-small">{{ project.description | truncate: 80 }}</p>
            
            <div class="project-features-small">
              {% if project.models %}
                <span class="feature-badge-small" title="3D Models">
                  <i class="fas fa-cube"></i>
                  {{ project.models.size }}
                </span>
              {% endif %}
              
              {% if project.schematics %}
                <span class="feature-badge-small" title="Schematics">
                  <i class="fas fa-microchip"></i>
                  {{ project.schematics.size }}
                </span>
              {% endif %}
              
              {% if project.code_files %}
                <span class="feature-badge-small" title="Code Files">
                  <i class="fas fa-code"></i>
                  {{ project.code_files.size }}
                </span>
              {% endif %}
            </div>
          </div>
        </div>
      {% endfor %}
    </div>
    
    <div class="showcase-actions">
      <a href="{{ '/projects/' | relative_url }}" class="btn-primary-large">
        <i class="fas fa-th"></i>
        View All Projects
      </a>
    </div>
  </div>
</div>

<div class="skills-section">
  <div class="container">
    <div class="skills-content">
      <h2>Technical Expertise</h2>
      <div class="skills-grid">
        <div class="skill-category">
          <h3><i class="fas fa-robot"></i> Robotics</h3>
          <div class="skill-tags">
            <span class="skill-tag">ROS2</span>
            <!-- <span class="skill-tag">Kinematics</span>
            <span class="skill-tag">Path Planning</span> -->
            <span class="skill-tag">SLAM</span>
            <span class="skill-tag">KUKA</span>
          </div>
        </div>
        <div class="skill-category">
          <h3><i class="fas fa-microchip"></i> Electronics</h3>
          <div class="skill-tags">
            <span class="skill-tag">Raspberry Pi</span>
            <span class="skill-tag">Arduino</span>
            <span class="skill-tag">ESP32</span>
            <span class="skill-tag">PCB Design</span>
            <!-- <span class="skill-tag">Sensors</span> -->
          </div>
        </div>
        <div class="skill-category">
          <h3><i class="fas fa-code"></i> Programming</h3>
          <div class="skill-tags">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">C/C++</span>
            <span class="skill-tag">MATLAB</span>
          </div>
        </div>
        <div class="skill-category">
          <h3><i class="fas fa-cube"></i> CAD/Design</h3>
          <div class="skill-tags">
            <span class="skill-tag">Fusion 360</span>
            <span class="skill-tag">3D Printing</span>
          </div>
        </div>
        <div class="skill-category">
          <h3><i class="fas fa-hexagon-nodes"></i> ML/AI</h3>
          <div class="skill-tags">
            <span class="skill-tag">Pytorch</span>
            <span class="skill-tag">mlflow</span>
            <span class="skill-tag">tensorboard</span>
            <span class="skill-tag">data science</span>
            <span class="skill-tag">Docker</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>