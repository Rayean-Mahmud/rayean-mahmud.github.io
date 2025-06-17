---
title: Support
layout: page
permalink: /support/
---

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap" rel="stylesheet">

<style>
  :root {
    --bg-color: #0d0d0d;
    --text-color: #fff;
    --card-bg: rgba(255, 255, 255, 0.05);
    --neon-accent: #ff00cc;
    --neon-alt: #00ffff;
    --border-color: #ff00cc;
  }

  [data-theme="light"] {
    --bg-color: #ffffff;
    --text-color: #000000;
    --card-bg: #f0f0f0;
    --neon-accent: #007acc;
    --neon-alt: #ff0077;
    --border-color: #007acc;
  }

  body {
    background-color: var(--bg-color);
    color: var(--text-color);
    font-family: 'Orbitron', sans-serif;
    transition: all 0.3s ease;
  }

  .support-card {
    max-width: 500px;
    margin: 30px auto;
    padding: 20px;
    border-radius: 15px;
    background: var(--card-bg);
    box-shadow: 0 0 20px var(--neon-alt);
    text-align: center;
    border: 1px solid var(--border-color);
  }

  .support-card h2 {
    font-size: 1.4rem;
    font-weight: bold;
    margin-bottom: 12px;
    color: var(--neon-accent);
    text-shadow: 0 0 5px var(--neon-alt);
  }

  .support-card p {
    margin-bottom: 10px;
    font-size: 0.95rem;
  }

  .support-card code {
    font-size: 1.2rem;
    background: rgba(255, 255, 255, 0.1);
    padding: 6px 12px;
    border-radius: 8px;
    color: var(--neon-accent);
    display: inline-block;
    margin-top: 5px;
    box-shadow: 0 0 5px var(--neon-accent);
  }

  .support-card img {
    max-width: 250px;
    margin: 15px auto 10px;
    display: block;
    border-radius: 10px;
    box-shadow: 0 0 12px var(--neon-alt);
  }

  .support-card .note {
    font-style: italic;
    color: #ccc;
    font-size: 0.85rem;
  }

  .btn-toggle {
    position: absolute;
    top: 1rem;
    right: 1rem;
    padding: 8px 16px;
    background-color: var(--neon-accent);
    color: black;
    font-weight: bold;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    box-shadow: 0 0 10px var(--neon-accent);
  }

  .btn-toggle:hover {
    background-color: var(--neon-alt);
    box-shadow: 0 0 15px var(--neon-alt);
  }
</style>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    const themeToggle = document.getElementById("theme-toggle");
    const root = document.documentElement;
    themeToggle.addEventListener("click", () => {
      const theme = root.getAttribute("data-theme") === "light" ? "dark" : "light";
      root.setAttribute("data-theme", theme);
      themeToggle.textContent = theme === "light" ? "🌙 Night Mode" : "☀️ Day Mode";
    });
  });
</script>

<div data-theme="dark" style="position: relative;">
  <button class="btn-toggle" id="theme-toggle">☀️ Day Mode</button>

  <div class="support-card">
    <h2>💜 Show Some Love</h2>

    <p>If you find my work helpful — whether it's an app, a blog post, or a design — you can support me directly via <strong>bKash</strong>.</p>

    <p style="font-size: 1.1rem;">
      📱 <strong>bKash Number:</strong><br>
      <code>01859-334307</code>
    </p>

    <img src="{{ site.baseurl }}/assets/images/bkash-qr.jpeg" alt="bKash QR Code">

    <p class="note">🙏 Your support means a lot and helps me keep creating awesome things.</p>
  </div>
</div>
