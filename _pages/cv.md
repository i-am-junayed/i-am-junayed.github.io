---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Download CV
[Click here to download my CV (PDF)](/assets/my_CV.pdf)

---

Education
======
<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

Work experience
======
<ul>{% for post in site.experience reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>
  
Skills
======
* Programming Languages
    * Python, C, C++
* Web Technologies
    * HTML 5, PHP, Javascript
* Computer skills
    * PyTorch, keras, C, C++, Advanced JAVA
* Database
    * SQL, MySQL, MongoDB

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
