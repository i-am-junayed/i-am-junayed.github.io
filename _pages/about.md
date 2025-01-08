---
permalink: /
title: "Welcome to my personal website.."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<div id="welcoming-text">
  <p id="english" style="display: inline;">Assalamualaikum and Welcome !! 
    Feel free to explore my projects, contributions, and ideas. I’m excited to share my work with you!</p>
  <p id="bangla" style="display: none;">আমার GitHub পেজে স্বাগতম! আমার প্রকল্প, অবদান, এবং ধারণাগুলি অন্বেষণ করতে বিনা দ্বিধায় আসুন। আমি আপনাদের সাথে আমার কাজ শেয়ার করতে উত্তেজিত!</p>
  <p id="french" style="display: none;">Bienvenue sur ma page GitHub! N'hésitez pas à explorer mes projets, mes contributions et mes idées. Je suis ravi de partager mon travail avec vous!</p>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function () {
    let currentLang = 0; // Start with English
    const languages = ['english', 'bangla', 'french'];

    function switchLanguage() {
      // Hide all paragraphs
      languages.forEach(lang => document.getElementById(lang).style.display = 'none');

      // Show the current language paragraph
      const currentParagraph = document.getElementById(languages[currentLang]);
      if (currentParagraph) {
        currentParagraph.style.display = 'inline';
      }

      // Update the currentLang index
      currentLang = (currentLang + 1) % languages.length;
    }

    // Set an interval to switch languages every 2 seconds
    setInterval(switchLanguage, 2000);

    // Initially call switchLanguage to show the first language immediately
    switchLanguage();
  });
</script>
