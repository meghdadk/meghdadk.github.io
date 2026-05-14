---
layout: page
title: news
permalink: /news/
nav: false
---

<style>
  .news-page {
    max-width: 960px;
  }

  .news-page-list {
    list-style: none;
    margin: 0;
    padding: 0;
    display: grid;
    gap: 0.95rem;
  }

  .news-page-item {
    display: grid;
    grid-template-columns: minmax(120px, 150px) minmax(0, 1fr);
    gap: 1rem;
    align-items: start;
    padding-bottom: 0.95rem;
    border-bottom: 1px solid rgba(22, 28, 45, 0.12);
  }

  .news-page-date {
    color: #788093;
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 0.06em;
    text-transform: uppercase;
  }

  .news-page-copy {
    font-size: 1rem;
    line-height: 1.7;
  }

  .news-page-copy a {
    font-weight: 600;
    text-decoration: none;
  }

  .news-page-copy a:hover {
    text-decoration: underline;
  }

  @media (max-width: 640px) {
    .news-page-item {
      grid-template-columns: 1fr;
      gap: 0.45rem;
    }
  }
</style>

<div class="news-page">
  <ol class="news-page-list">
    {% assign sorted_news = site.news | sort: "date" | reverse %}
    {% for item in sorted_news %}
      <li class="news-page-item">
        <span class="news-page-date">{{ item.date | date: "%B %Y" }}</span>
        <div class="news-page-copy">{{ item.content }}</div>
      </li>
    {% endfor %}
  </ol>
</div>
