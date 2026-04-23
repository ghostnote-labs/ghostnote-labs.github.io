---
layout: default
permalink: /
title:
---
<!--
  Landing page for ghostnotelabs.studio. Kept as raw HTML (no
  markdown body) so the styling lines up exactly with what the
  default layout provides — no auto-wrapping of prose in <p> tags
  that would fight the .home flex layout.

  Front matter MUST be the very first characters in this file.
  Any content before the opening --- (including HTML comments)
  causes Jekyll to skip parsing and render the YAML as literal
  text in the page body.
-->

<section class="home">
  <img class="home-logo" src="{{ '/assets/logo.svg' | relative_url }}" alt="Ghostnote Labs">

  <h1>GHOSTNOTE LABS</h1>

  <p class="home-tagline">
    A small software studio in Portland, Oregon, building craft-focused consumer products.
  </p>

  <p class="home-sub">
    Our first project is a fitness role-playing game, currently in private alpha with a closed cohort of testers. More when it's ready.
  </p>

  <p class="home-contact">
    <a href="mailto:ghostnotelabsllc@gmail.com">ghostnotelabsllc@gmail.com</a>
  </p>
</section>
