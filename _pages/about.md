---
layout: about
title: about
permalink: /
nav: true
nav_order: 1
subtitle: AI Research Scientist at IQVIA | Visiting Researcher at University of Cambridge
news: false
selected_papers: false
social: false
---
<style>
  :root {
    --home-bg: #efefef;
    --home-bg-deep: #e6e6e6;
    --home-surface: rgba(255, 255, 255, 0.76);
    --home-surface-strong: rgba(255, 255, 255, 0.92);
    --home-border: rgba(22, 28, 45, 0.12);
    --home-border-strong: rgba(22, 28, 45, 0.18);
    --home-text: #171b26;
    --home-muted: #5c6475;
    --home-soft: #788093;
    --home-shadow: 0 18px 42px rgba(22, 28, 45, 0.06);
  }

  html[data-theme="dark"] {
    --home-bg: #14171d;
    --home-surface: rgba(24, 28, 36, 0.78);
    --home-surface-strong: rgba(31, 36, 46, 0.92);
    --home-border: rgba(233, 238, 248, 0.12);
    --home-border-strong: rgba(233, 238, 248, 0.18);
    --home-text: #edf2fb;
    --home-muted: #bcc6d8;
    --home-soft: #96a3bb;
    --home-grid: rgba(233, 238, 248, 0.05);
    --home-shadow: 0 18px 42px rgba(0, 0, 0, 0.32);
  }

  body.sticky-bottom-footer {
    background-color: var(--home-bg);
    background-image:
      radial-gradient(circle at top center, rgba(255, 255, 255, 0.78) 0, rgba(255, 255, 255, 0.78) 18%, rgba(255, 255, 255, 0) 48%),
      radial-gradient(circle at top left, rgba(255, 255, 255, 0.42) 0, rgba(255, 255, 255, 0) 34%),
      linear-gradient(180deg, #f4f4f4 0%, var(--home-bg) 38%, var(--home-bg-deep) 100%);
    background-attachment: fixed;
    color: var(--home-text);
  }

  html[data-theme="dark"] body.sticky-bottom-footer {
    background:
      linear-gradient(var(--home-grid) 1px, transparent 1px),
      linear-gradient(90deg, var(--home-grid) 1px, transparent 1px),
      linear-gradient(180deg, #101318 0%, var(--home-bg) 100%);
  }

  .container.mt-5 {
    max-width: 1360px;
    padding-left: 2rem;
    padding-right: 2rem;
  }

  .post {
    max-width: 100%;
  }

  .post-header {
    margin: 3.25rem auto 2.5rem;
    max-width: 1100px;
    padding-bottom: 2rem;
    border-bottom: 1px solid var(--home-border);
  }

  .post-title {
    margin-bottom: 0.45rem;
    color: var(--home-text);
    font-size: clamp(1.7rem, 3.2vw, 2.55rem);
    line-height: 1.08;
    letter-spacing: -0.02em;
  }

  .post-header .desc {
    color: var(--home-muted) !important;
    font-size: 1.08rem;
  }

  .homepage-shell {
    max-width: 1100px;
    margin: 0 auto 4rem;
  }

  .home-card {
    position: relative;
    border: 1px solid var(--home-border-strong);
    border-radius: 24px;
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.92) 0%, rgba(251, 251, 251, 0.76) 100%);
    box-shadow: var(--home-shadow);
  }

  html[data-theme="dark"] .home-card {
    background:
      radial-gradient(circle at top left, rgba(39, 46, 58, 0.96), rgba(24, 28, 36, 0.82) 55%, rgba(18, 21, 27, 0.92) 100%);
  }

  .home-hero {
    display: grid;
    grid-template-columns: minmax(0, 1.45fr) minmax(280px, 0.78fr);
    gap: 1.7rem;
    padding: 1.4rem;
    margin-bottom: 2.2rem;
  }

  .home-hero-copy {
    padding: 0.1rem 0.2rem 0.1rem 0.15rem;
  }

  .home-kicker {
    margin: 0 0 1rem;
    color: var(--home-soft);
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .home-hero-title {
    margin: 0 0 1.15rem;
    color: var(--home-text);
    font-size: clamp(1.55rem, 3.5vw, 2.4rem);
    line-height: 1.2;
    letter-spacing: -0.01em;
  }

  .home-hero-copy p {
    margin: 0 0 0.9rem;
    color: var(--home-muted);
    font-size: 0.97rem;
    line-height: 1.72;
    max-width: 36rem;
  }

  .home-pill-row {
    display: flex;
    flex-wrap: wrap;
    gap: 0.65rem;
    margin-top: 1.35rem;
  }

  .home-pill,
  .home-pill:visited {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-height: 2.95rem;
    padding: 0.72rem 1rem;
    border: 1px solid var(--home-border-strong);
    border-radius: 999px;
    background: var(--home-surface);
    color: var(--home-text);
    font-size: 0.92rem;
    font-weight: 600;
    text-decoration: none;
    transition: transform 0.18s ease, background 0.18s ease, border-color 0.18s ease;
  }

  .home-pill:hover {
    transform: translateY(-1px);
    background: var(--home-surface-strong);
    border-color: rgba(22, 28, 45, 0.24);
  }

  html[data-theme="dark"] .home-pill:hover {
    border-color: rgba(233, 238, 248, 0.22);
  }

  .home-hero-visual {
    display: flex;
    align-items: stretch;
  }

  .home-portrait {
    width: 100%;
    height: 100%;
    min-height: 430px;
    object-fit: cover;
    border-radius: 18px;
    filter: grayscale(100%);
    border: 1px solid var(--home-border);
  }

  .home-section {
    margin-top: 2.5rem;
    padding-top: 2rem;
    border-top: 1px solid var(--home-border);
  }

  .home-section h2 {
    margin: 0 0 1.45rem;
    color: var(--home-text);
    font-size: clamp(1.85rem, 3vw, 2.65rem);
    line-height: 1.04;
    letter-spacing: -0.04em;
  }

  .news-shell {
    display: grid;
    gap: 1.1rem;
  }

  .news-list {
    list-style: none;
    margin: 0;
    padding: 0;
    display: grid;
    gap: 0.8rem;
  }

  .news-item {
    display: grid;
    grid-template-columns: minmax(120px, 150px) minmax(0, 1fr);
    gap: 1rem;
    align-items: start;
    padding-bottom: 0.8rem;
    border-bottom: 1px solid var(--home-border);
  }

  .news-date {
    display: inline-block;
    align-self: start;
    color: var(--home-soft);
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 0.06em;
    text-transform: uppercase;
  }

  .news-copy {
    color: var(--home-muted);
    font-size: 0.95rem;
    line-height: 1.65;
  }

  .news-copy a {
    color: var(--home-text);
    font-weight: 600;
    text-decoration: none;
  }

  .news-copy a:hover {
    text-decoration: underline;
  }

  .news-link,
  .news-link:visited {
    display: inline-flex;
    align-items: center;
    padding: 0.72rem 1rem;
    border: 1px solid var(--home-border-strong);
    border-radius: 999px;
    background: var(--home-surface);
    color: var(--home-text);
    font-size: 0.92rem;
    font-weight: 600;
    text-decoration: none;
    transition: transform 0.18s ease, background 0.18s ease, border-color 0.18s ease;
  }

  .news-link:hover {
    transform: translateY(-1px);
    background: var(--home-surface-strong);
    border-color: rgba(22, 28, 45, 0.24);
  }

  html[data-theme="dark"] .news-link:hover {
    border-color: rgba(233, 238, 248, 0.22);
  }

  .home-publications {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
  }

  .publication-card {
    display: flex;
    flex-direction: column;
    min-height: 100%;
    padding: 1rem 1.05rem 1.1rem;
    border: 1px solid var(--home-border);
    border-radius: 18px;
    background: var(--home-surface);
    box-shadow: 0 12px 30px rgba(22, 28, 45, 0.04);
  }

  html[data-theme="dark"] .publication-card {
    box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
  }

  .publication-card h3,
  .publication-card h3 a {
    margin: 0;
    color: var(--home-text);
    font-size: 1.08rem;
    line-height: 1.18;
    letter-spacing: -0.03em;
    text-decoration: none;
  }

  .publication-badge {
    display: inline-flex;
    align-self: flex-start;
    margin: 0.85rem 0 0.95rem;
    padding: 0.42rem 0.7rem;
    border: 1px solid var(--home-border-strong);
    border-radius: 10px;
    background: var(--home-surface-strong);
    color: var(--home-text);
    font-size: 0.81rem;
    font-weight: 700;
  }

  .publication-authors {
    margin: 0 0 0.95rem;
    color: var(--home-soft);
    font-size: 0.88rem;
    line-height: 1.48;
  }

  .publication-summary {
    margin: 0 0 1rem;
    color: var(--home-muted);
    font-size: 0.93rem;
    line-height: 1.6;
  }

  .publication-links {
    margin-top: auto;
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
  }

  .publication-links a {
    color: var(--home-muted);
    font-weight: 600;
    text-decoration: none;
  }

  .publication-links a:hover {
    color: var(--home-text);
  }

  .publication-card.publication-card-wide {
    display: grid;
    place-items: center;
    min-height: 260px;
    text-align: center;
  }

  .publication-card.publication-card-wide a {
    color: var(--home-text);
    text-decoration: none;
    font-size: clamp(1.55rem, 2.4vw, 2.05rem);
    line-height: 1.05;
    letter-spacing: -0.04em;
    font-weight: 700;
  }

  footer.fixed-bottom {
    background: transparent !important;
  }

  @media (max-width: 1024px) {
    .home-hero,
    .home-publications {
      grid-template-columns: 1fr;
    }

    .home-portrait {
      min-height: 360px;
    }
  }

  @media (max-width: 640px) {
    .container.mt-5 {
      padding-left: 1rem;
      padding-right: 1rem;
    }

    .post-header {
      margin-top: 2.2rem;
    }

    .home-hero {
      padding: 1rem;
      gap: 1rem;
    }

    .home-hero-title {
      font-size: 1.72rem;
    }

    .home-pill {
      width: 100%;
    }

    .publication-card {
      padding: 1rem;
    }

    .news-item {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="homepage-shell">
  <section class="home-card home-hero">
    <div class="home-hero-copy">
      <p class="home-kicker">AI Research Scientist</p>
      <h2 class="home-hero-title">AI Scientist building scalable generative AI systems</h2>
      <p>
        I work across the full machine learning lifecycle, from designing new models to building production-grade
        pipelines for enterprise AI systems. My recent work spans large-scale model training, multimodal learning,
        agentic LLM systems, and safety-critical AI.
      </p>
      <p>
        My research has focused on machine unlearning, decentralized LLM pre-training, privacy-preserving learning,
        and AI safety, with publications in venues including NeurIPS, ICLR, and SIGMOD and funded work on
        privacy-preserving and safety-critical machine learning systems.
      </p>

      <div class="home-pill-row">
        <a class="home-pill" href="mailto:mk2296@cam.ac.uk">Email</a>
        <a class="home-pill" href="/assets/pdf/CV.pdf">CV</a>
        <a class="home-pill" href="https://scholar.google.com/citations?user=7t9HbecAAAAJ&hl=en">Google Scholar</a>
        <a class="home-pill" href="https://github.com/meghdadk">GitHub</a>
        <a class="home-pill" href="https://www.linkedin.com/in/meghdad-kurmanji-948380113/">LinkedIn</a>
        <a class="home-pill" href="https://x.com/meghdadkurmanji">X</a>
      </div>
    </div>

    <div class="home-hero-visual">
      <img class="home-portrait" src="/assets/images/profile_photo.jpeg" alt="Portrait of Meghdad Kurmanji">
    </div>
  </section>

  <section class="home-section">
    <h2>News</h2>

    <div class="news-shell">
      <ol class="news-list">
        <li class="news-item">
          <span class="news-date">January 2026</span>
          <div class="news-copy">I started a new position as an AI Scientist at IQVIA.</div>
        </li>
        <li class="news-item">
          <span class="news-date">January 2026</span>
          <div class="news-copy">
            Two papers got accepted to ICLR 2026:
            <a href="https://arxiv.org/pdf/2510.05361">PDF 1</a>,
            <a href="https://arxiv.org/pdf/2505.22549">PDF 2</a>.
          </div>
        </li>
        <li class="news-item">
          <span class="news-date">January 2026</span>
          <div class="news-copy">
            Our proposal received a GBP 150k grant through Foresight's AI Safety call. We will use interpretability to enable precise unlearning, even in challenging scenarios.
          </div>
        </li>
        <li class="news-item">
          <span class="news-date">December 2025</span>
          <div class="news-copy">I attended NeurIPS in Copenhagen and presented 2 posters and 2 oral talks.</div>
        </li>
        <li class="news-item">
          <span class="news-date">November 2025</span>
          <div class="news-copy">
            One paper was accepted at AAAI's Alignment Track:
            <a href="https://openreview.net/forum?id=naUNy565N9#discussion">link</a>.
          </div>
        </li>
      </ol>
      <a class="news-link" href="/news/">View all news</a>
    </div>
  </section>

  <section class="home-section">
    <h2>Selected Publications</h2>

    <div class="home-publications">
      <article class="publication-card">
        <h3><a href="https://openreview.net/forum?id=5A7xphgC0V">DEPT: Decoupled Embeddings for Pre-training Language Models</a></h3>
        <span class="publication-badge">ICLR 2025</span>
        <p class="publication-authors">Meghdad Kurmanji et al.</p>
        <p class="publication-summary">Research on pre-training language models with decoupled embeddings, recognized among the top 1 percent of submissions.</p>
        <div class="publication-links">
          <a href="https://openreview.net/forum?id=5A7xphgC0V">Paper</a>
        </div>
      </article>

      <article class="publication-card">
        <h3><a href="https://arxiv.org/pdf/2502.12430">Bridge the Gaps between Machine Unlearning and AI Regulation</a></h3>
        <span class="publication-badge">NeurIPS 2025</span>
        <p class="publication-authors">Bill Marino, Meghdad Kurmanji, Nicholas D. Lane</p>
        <p class="publication-summary">Connects machine unlearning research with regulatory requirements and highlights the gap between current technical methods and compliance needs in practice.</p>
        <div class="publication-links">
          <a href="https://arxiv.org/pdf/2502.12430">PDF</a>
        </div>
      </article>

      <article class="publication-card">
        <h3><a href="https://arxiv.org/pdf/2406.01257">What Makes Unlearning Hard and What to Do About It</a></h3>
        <span class="publication-badge">NeurIPS 2024</span>
        <p class="publication-authors">Kai Zhao, Meghdad Kurmanji, George Barbulescu, Efi Triantafillou, Peter Triantafillou</p>
        <p class="publication-summary">Studies the core obstacles behind effective unlearning and lays out practical directions for building more reliable removal methods under real utility constraints.</p>
        <div class="publication-links">
          <a href="https://arxiv.org/pdf/2406.01257">PDF</a>
        </div>
      </article>

      <article class="publication-card">
        <h3><a href="https://dl.acm.org/doi/pdf/10.1145/3639304">Machine Unlearning in Learned Databases</a></h3>
        <span class="publication-badge">SIGMOD 2024</span>
        <p class="publication-authors">Meghdad Kurmanji, Efi Triantafillou, Peter Triantafillou</p>
        <p class="publication-summary">Introduces unlearning in learned database systems and shows how removal requirements interact with approximation, indexing, and database-facing model maintenance.</p>
        <div class="publication-links">
          <a href="https://dl.acm.org/doi/pdf/10.1145/3639304">PDF</a>
        </div>
      </article>

      <article class="publication-card">
        <h3><a href="https://arxiv.org/pdf/2302.09880.pdf">Towards Unbounded Machine Unlearning</a></h3>
        <span class="publication-badge">NeurIPS 2023</span>
        <p class="publication-authors">Meghdad Kurmanji, Peter Triantafillou, Jamie Hayes, Efi Triantafillou</p>
        <p class="publication-summary">Explores scalable unlearning beyond narrow one-shot settings, focusing on repeated removal requests and stable model performance over time.</p>
        <div class="publication-links">
          <a href="https://arxiv.org/pdf/2302.09880.pdf">PDF</a>
        </div>
      </article>

      <article class="publication-card publication-card-wide">
        <a href="/publications/">Full Bibliography</a>
      </article>
    </div>
  </section>
</div>
