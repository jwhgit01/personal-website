---
layout: default
title: Publications
permalink: /publications/
---

# Publications
*See [Google Scholar](https://scholar.google.com/citations?hl=en&user=-kIX4SIAAAAJ) for an up-to-date list of publications.* 

{% bibliography %}

<script>
document.addEventListener("DOMContentLoaded", function() {
  const buttons = document.querySelectorAll('.pdf-download-btn');
  buttons.forEach(function(btn) {
    fetch(btn.dataset.pdf, { method: 'HEAD' }).then(function(resp) {
      if (!resp.ok) {
        btn.style.display = 'none';
      }
    }).catch(function() {
      btn.style.display = 'none';
    });
  });
});
</script>
