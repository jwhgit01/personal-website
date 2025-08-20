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

function toggleExclusive(sectionId, entryKey) {
  // Get the abstract and bibtex elements
  var abstract = document.getElementById(entryKey + '_abstract');
  var bibtex = document.getElementById(entryKey + '_bibtex');

  // Get the selected section
  var selected = document.getElementById(sectionId);

  // If the selected section is open, close it
  if (selected && selected.style.display === "block") {
    selected.style.display = "none";
  } else {
    // Otherwise, hide both and show the selected one
    if (abstract) abstract.style.display = 'none';
    if (bibtex) bibtex.style.display = 'none';

    // Show the selected section
    if (selected) selected.style.display = 'block';
  }
}
</script>
