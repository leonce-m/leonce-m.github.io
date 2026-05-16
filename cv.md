---
layout: default
title: "CV"
permalink: /cv/
---

<main class="cv-viewer" aria-label="CV">
  <div class="cv-viewer__pages">
    {% assign cv_pages = site.static_files | where_exp: "file", "file.path contains '/assets/cv/pages/'" | sort: "path" %}
    {% for page in cv_pages %}
      <img
        class="cv-viewer__page"
        src="{{ page.path | relative_url }}"
        alt="CV page {{ forloop.index }}"
      >
    {% endfor %}
  </div>
  <p class="cv-viewer__pdf-link">
    <a href="/assets/cv/cv_leonce_mollerus.pdf">Open as PDF</a>
  </p>
</main>
