<!--
  Landing page for ghostnotelabs.studio.

  The default layout switches on page.url == "/" and injects this
  content directly (without the doc-page header/footer wrapper). All
  markup here is the hero/landing content itself.

  Keep this file HTML-only (no markdown) so the site renders exactly
  as styled, without Kindle/Jekyll wrapping prose in <p> tags that
  would fight the layout.
-->
---
layout: default
permalink: /
title:
---

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
