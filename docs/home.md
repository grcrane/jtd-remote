---
layout: default
title: Home
nav_order: 1
description: "Documentation for the UIL SquareSpace website development team."
permalink: /
---

# UIL Website Documentation

Just the Docs gives your documentation a jumpstart with a responsive Jekyll theme that is easily customizable and hosted on GitHub Pages.

---

## Getting started

## Dependencies

## George handy links and such

**pretty print variables**
`
<pre id="jekyll-debug"></pre>
<script>
  var obj = JSON.parse(decodeURIComponent("{{ site | jsonify | uri_escape }}"));
  var prettyJson = JSON.stringify(obj, null, 4);  // Pretty-printed JSON (indented 4 spaces).
  document.getElementById("jekyll-debug").textContent = prettyJson;
</script>
`