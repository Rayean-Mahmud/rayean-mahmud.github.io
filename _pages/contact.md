---
title: "Contact"
permalink: "/contact.html"
layout: page
---

<!-- ✅ Mailchimp Sitewide Script (paste in <head> section of your layout if not already) -->
<script id="mcjs">
!function(c,h,i,m,p){m=c.createElement(h),
p=c.getElementsByTagName(h)[0],m.async=1,m.src=i,
p.parentNode.insertBefore(m,p)}
(document,"script","https://chimpstatic.com/mcjs-connected/js/users/aa6e06d3ca4533f339ea0783b/f4a44c943af3b3947b766e8a7.js");
</script>

<style>
  .contact-form, .newsletter-form {
    max-width: 600px;
    margin: 2rem auto;
    padding: 2rem;
    background-color: #f9f9f9;
    border-radius: 12px;
    box-shadow: 0 0 10px rgba(0,0,0,0.05);
  }

  .contact-form h2, .newsletter-form h2 {
    text-align: center;
    margin-bottom: 1.5rem;
  }

  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 600;
  }

  input, textarea {
    width: 100%;
    padding: 0.75rem;
    margin-bottom: 1.2rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
  }

  button {
    width: 100%;
    padding: 0.75rem;
    font-size: 1.1rem;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  .contact-form button {
    background-color: #007bff;
    color: #fff;
  }

  .contact-form button:hover {
    background-color: #0056b3;
  }

  .newsletter-form button {
    background-color: #28a745;
    color: #fff;
  }

  .newsletter-form button:hover {
    background-color: #1e7e34;
  }
</style>

<!-- 📬 Contact Form -->
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

<!-- 📰 Newsletter Signup (Mailchimp Embedded Form) -->
<div class="newsletter-form">
  <h2>📨 Subscribe to Newsletter</h2>
  <form action="https://us14.list-manage.com/subscribe/post?u=aa6e06d3ca4533f339ea0783b&amp;id=f4a44c943a" method="post" target="_self" novalidate>
    <input type="email" name="EMAIL" placeholder="Enter your email" required>
    <button type="submit">Subscribe</button>
  </form>
</div>



    <label for="message">Your Message</label>
    <textarea name="message" id="message" rows="6" placeholder="Write your message here..." required></textarea>

    <button type="submit">Send Message</button>
  </form>
</div>
