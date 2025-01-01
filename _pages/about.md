---
permalink: /
title: "Welcome to my personal website.."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div id="welcoming-text">
  <p id="english" style="display: inline;">Welcome to my GitHub page! Feel free to explore my projects, contributions, and ideas. I’m excited to share my work with you!</p>
  <p id="bangla" style="display: none;">আমার GitHub পেজে স্বাগতম! আমার প্রকল্প, অবদান, এবং ধারণাগুলি অন্বেষণ করতে বিনা দ্বিধায় আসুন। আমি আপনাদের সাথে আমার কাজ শেয়ার করতে উত্তেজিত!</p>
  <p id="french" style="display: none;">Bienvenue sur ma page GitHub! N'hésitez pas à explorer mes projets, mes contributions et mes idées. Je suis ravi de partager mon travail avec vous!</p>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    let currentLang = 0; // Start with English
    const languages = ['english', 'bangla', 'french'];
    
    setInterval(function () {
      // Hide all paragraphs
      languages.forEach(lang => document.getElementById(lang).style.display = 'none');
      
      // Show the current language paragraph
      document.getElementById(languages[currentLang]).style.display = 'inline';
      
      // Update the currentLang index
      currentLang = (currentLang + 1) % languages.length;
    }, 1000); // Switch language every 1 second
  });
</script>
