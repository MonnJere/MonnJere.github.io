---
layout: page
title:  ""
permalink: /contact/
header:
  title: Contact Me
  image_fullwidth: header_unsplash_4.jpg     # 1600×503 banner (optional)
sidebar: none
---

<section class="contact-hero text-center">
  <h1>Let’s Connect</h1>
  <p class="lead">
    Have a project in mind, a question about my work, or just want to say
    hello? Drop a line- I usually reply within a couple business day.
  </p>
</section>

<!-- ── CONTACT FORM ───────────────────────────────────────────── -->
<form
  action="https://formspree.io/f/mldbwona"
  method="POST"
>
  <div class="row">
    <div class="medium-6 columns">
      <label>Name
        <input type="text" name="name" placeholder="Your name" required>
      </label>
    </div>

    <div class="medium-6 columns">
      <label>Email
        <input type="email" name="email" placeholder="your@email.com"
               required>
      </label>
    </div>
  </div>

  <label>Subject
    <input type="text" name="_subject" placeholder="How can I help?" required>
  </label>

  <label>Message
    <textarea name="message" rows="6" placeholder="" required></textarea>
  </label>

  <!-- honeypot field (spam blocker) -->
  <input type="text" name="_gotcha" style="display:none">

  <!-- success redirect -->
  <input type="hidden" name="_next" value="{{ '/thanks/' | relative_url }}">

  <button type="submit" class="button radius">Send&nbsp;Message →</button>
</form>
