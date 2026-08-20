<div align="center">

<!-- Animated Header -->
<style>
  @keyframes slideIn {
    from {
      opacity: 0;
      transform: translateY(-20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  @keyframes glow {
    0%, 100% {
      text-shadow: 0 0 10px rgba(59, 130, 246, 0.5);
    }
    50% {
      text-shadow: 0 0 20px rgba(59, 130, 246, 0.8);
    }
  }

  @keyframes float {
    0%, 100% {
      transform: translateY(0px);
    }
    50% {
      transform: translateY(-10px);
    }
  }

  @keyframes rotate {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(360deg);
    }
  }

  .header-title {
    animation: slideIn 0.8s ease-out, glow 2s ease-in-out infinite;
    font-size: 3em;
    font-weight: 800;
    background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 50%, #ec4899 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
  }

  .subtitle {
    animation: slideIn 0.8s ease-out 0.2s both;
    font-size: 1.3em;
    color: #666;
    margin-bottom: 30px;
  }

  .badge-container {
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
    margin-bottom: 40px;
    animation: slideIn 0.8s ease-out 0.4s both;
  }

  .badge {
    display: inline-block;
    padding: 8px 16px;
    background: linear-gradient(135deg, #3b82f6, #8b5cf6);
    color: white;
    border-radius: 20px;
    font-weight: 600;
    font-size: 0.9em;
    transition: all 0.3s ease;
  }

  .badge:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 25px rgba(59, 130, 246, 0.3);
  }

  .divider {
    width: 100px;
    height: 4px;
    background: linear-gradient(90deg, #3b82f6, #8b5cf6, #ec4899);
    margin: 40px auto;
    border-radius: 2px;
    animation: slideIn 0.8s ease-out 0.6s both;
  }

  .section-title {
    font-size: 1.8em;
    font-weight: 700;
    color: #1f2937;
    margin-bottom: 20px;
    text-align: left;
    animation: slideIn 0.6s ease-out both;
  }

  .tech-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
    gap: 15px;
    margin: 30px 0;
  }

  .tech-item {
    padding: 15px;
    background: linear-gradient(135deg, #f0f9ff, #f5f3ff);
    border: 2px solid #e0e7ff;
    border-radius: 10px;
    text-align: center;
    transition: all 0.3s ease;
    font-weight: 600;
    color: #4f46e5;
  }

  .tech-item:hover {
    transform: translateY(-8px);
    border-color: #3b82f6;
    box-shadow: 0 15px 30px rgba(59, 130, 246, 0.2);
    background: linear-gradient(135deg, #dbeafe, #ede9fe);
  }

  .stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
    gap: 20px;
    margin: 30px 0;
  }

  .stat-card {
    padding: 25px;
    background: linear-gradient(135deg, #ffffff, #f9fafb);
    border: 2px solid #e5e7eb;
    border-radius: 12px;
    text-align: center;
    transition: all 0.3s ease;
  }

  .stat-card:hover {
    transform: translateY(-8px);
    border-color: #3b82f6;
    box-shadow: 0 20px 40px rgba(59, 130, 246, 0.15);
  }

  .stat-number {
    font-size: 2.5em;
    font-weight: 800;
    background: linear-gradient(135deg, #3b82f6, #8b5cf6);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .stat-label {
    font-size: 0.9em;
    color: #666;
    margin-top: 8px;
  }

  .project-card {
    text-align: left;
    padding: 20px;
    background: linear-gradient(135deg, #ffffff, #f9fafb);
    border: 2px solid #e5e7eb;
    border-radius: 12px;
    margin: 15px 0;
    transition: all 0.3s ease;
  }

  .project-card:hover {
    transform: translateX(8px);
    border-color: #3b82f6;
    box-shadow: 0 15px 35px rgba(59, 130, 246, 0.15);
  }

  .project-title {
    font-size: 1.3em;
    font-weight: 700;
    color: #1f2937;
    margin-bottom: 8px;
  }

  .project-desc {
    color: #666;
    font-size: 0.95em;
    margin-bottom: 12px;
  }

  .project-tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
  }

  .tag {
    display: inline-block;
    padding: 4px 12px;
    background: #e0e7ff;
    color: #4f46e5;
    border-radius: 15px;
    font-size: 0.8em;
    font-weight: 600;
  }

  .contact-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin: 40px 0;
    flex-wrap: wrap;
  }

  .contact-link {
    padding: 12px 24px;
    background: linear-gradient(135deg, #3b82f6, #8b5cf6);
    color: white;
    text-decoration: none;
    border-radius: 8px;
    font-weight: 600;
    transition: all 0.3s ease;
    display: inline-block;
  }

  .contact-link:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 30px rgba(59, 130, 246, 0.3);
  }

  .footer-note {
    margin-top: 50px;
    padding-top: 30px;
    border-top: 2px solid #e5e7eb;
    color: #999;
    font-size: 0.9em;
  }
</style>

<h1 class="header-title">Arthur Candian Rocha</h1>
<p class="subtitle">💻 Developer | 🚀 Builder | ✨ Innovator</p>

<div class="badge-container">
  <span class="badge">Full-Stack Developer</span>
  <span class="badge">UI/UX Enthusiast</span>
  <span class="badge">Problem Solver</span>
</div>

<div class="divider"></div>

</div>

## 🎯 Sobre Mim

Desenvolvedor apaixonado por criar soluções inovadoras e elegantes. Especializado em desenvolvimento full-stack com foco em experiência do usuário e design de interfaces. Sempre buscando aprender novas tecnologias e melhorar minhas habilidades.

<div align="center">

### 📊 Estatísticas

</div>

<div class="stats-grid">
  <div class="stat-card">
    <div class="stat-number">5+</div>
    <div class="stat-label">Anos de Experiência</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">50+</div>
    <div class="stat-label">Projetos Completados</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">15+</div>
    <div class="stat-label">Tecnologias</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">100%</div>
    <div class="stat-label">Dedicação</div>
  </div>
</div>

---

## 🛠️ Tech Stack

<div class="tech-grid">
  <div class="tech-item">JavaScript</div>
  <div class="tech-item">TypeScript</div>
  <div class="tech-item">React</div>
  <div class="tech-item">Node.js</div>
  <div class="tech-item">Python</div>
  <div class="tech-item">SQL</div>
  <div class="tech-item">HTML/CSS</div>
  <div class="tech-item">Git</div>
  <div class="tech-item">Docker</div>
  <div class="tech-item">AWS</div>
  <div class="tech-item">PostgreSQL</div>
  <div class="tech-item">MongoDB</div>
</div>

---

## 🚀 Projetos Destaque

<div class="project-card">
  <div class="project-title">📱 Projeto 1 - APP Mobile</div>
  <div class="project-desc">Aplicação mobile inovadora com design intuitivo e performance otimizada.</div>
  <div class="project-tags">
    <span class="tag">React Native</span>
    <span class="tag">Firebase</span>
    <span class="tag">UI/UX</span>
  </div>
</div>

<div class="project-card">
  <div class="project-title">🌐 Projeto 2 - Web Platform</div>
  <div class="project-desc">Plataforma web escalável com arquitetura moderna e componentes reutilizáveis.</div>
  <div class="project-tags">
    <span class="tag">Next.js</span>
    <span class="tag">TypeScript</span>
    <span class="tag">TailwindCSS</span>
  </div>
</div>

<div class="project-card">
  <div class="project-title">⚡ Projeto 3 - API Backend</div>
  <div class="project-desc">API robusta com autenticação, validação e testes automatizados.</div>
  <div class="project-tags">
    <span class="tag">Node.js</span>
    <span class="tag">Express</span>
    <span class="tag">PostgreSQL</span>
  </div>
</div>

---

<div align="center">

## 💬 Vamos Conectar!

</div>

<div class="contact-links">
  <a href="https://linkedin.com/in/arthurrocha" class="contact-link">🔗 LinkedIn</a>
  <a href="mailto:seu.email@exemplo.com" class="contact-link">📧 Email</a>
  <a href="https://twitter.com/arthurrocha" class="contact-link">🐦 Twitter</a>
  <a href="https://portfolio.seu-site.com" class="contact-link">🌐 Portfólio</a>
</div>

<div align="center">

---

<div class="footer-note">
  ⭐ Se gostou, deixa uma estrela nos repos! | Sempre aberto para colaborações e oportunidades incríveis.
</div>

</div>
