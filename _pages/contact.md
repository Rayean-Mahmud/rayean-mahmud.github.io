---
title: "Contact"
permalink: "/contact.html"
layout: page
---

<style>
  .contact-form {
    max-width: 600px;
    margin: 2rem auto;
    padding: 2rem;
    background-color: #f9f9f9;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0,0,0,0.05);
  }

  .contact-form h2 {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  .contact-form label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 600;
  }

  .contact-form input,
  .contact-form textarea {
    width: 100%;
    padding: 0.75rem;
    margin-bottom: 1.2rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
  }

  .contact-form button {
    width: 100%;
    padding: 0.75rem;
    background-color: #007bff;
    color: #fff;
    font-size: 1.1rem;
    border: none;
    border-radius: 8px;
    cursor: pointer;
  }

  .contact-form button:hover {
    background-color: #0056b3;
  }

  .newsletter-form {
    max-width: 600px;
    margin: 2rem auto;
    padding: 2rem;
    background-color: #f1f1f1;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0,0,0,0.05);
  }

  .newsletter-form h2 {
    text-align: center;
    margin-bottom: 1.2rem;
  }

  .newsletter-form input {
    width: 100%;
    padding: 0.75rem;
    margin-bottom: 1rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
  }

  .newsletter-form button {
    width: 100%;
    padding: 0.75rem;
    background-color: #28a745;
    color: #fff;
    font-size: 1.1rem;
    border: none;
    border-radius: 8px;
    cursor: pointer;
  }

  .newsletter-form button:hover {
    background-color: #218838;
  }
</style>

<!-- Contact Form -->
<div class="contact-form">
  <h2>📬 Get in Touch</h2>
  <form action="https://formspree.io/f/xovwdvzk" method="POST">
    <label for="email">Your Email</label>
    <input type="email" name="email" id="email" placeholder="you@example.com" required>

    <label for="message">Your Message</label>
    <textarea name="message" id="message" rows="6" placeholder="Write your message here..." required></textarea>

    <button type="submit">Send Message</button>
  </form>
</div>

<!-- Newsletter Form -->
<div class="newsletter-form">
  <h2>📨 Subscribe to Newsletter</h2>
  <form action="https://formsubmit.co/rayean.dev@gmail.com" method="POST">
    <input type="email" name="email" placeholder="Enter your email to subscribe" required>
    
    <!-- Prevent bot signups -->
    <input type="text" name="_honey" style="display:none">
    <!-- No captcha -->
    <input type="hidden" name="_captcha" value="false">
    <!-- Redirect after success (optional) -->
    <input type="hidden" name="_next" value="https://yourdomain.com/thank-you.html">

    <button type="submit">Subscribe</button>
  </form>
</div>


    <label for="message">Your Message</label>
    <textarea name="message" id="message" rows="6" placeholder="Write your message here..." required></textarea>

    <button type="submit">Send Message</button>
  </form>
</div>
