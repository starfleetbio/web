---
title: "DNAVault"
layout: splash
permalink: /dnavault/
dnavault_site: true
show_date: false
header:
  overlay_image: /assets/images/header.jpg
  overlay_filter: 0.5
  overlay_color: "#0D1117"
  og_image: /assets/images/logo.png
  actions:
    - label: "Download on the App Store"
      url: "https://apps.apple.com/app/dnavault/id6741454239"
      btn_class: "btn--primary btn--large"
excerpt: >
  Your genome is encrypted with a key that only your phone holds.<br>
  <small>We process your DNA inside a cryptographically attested enclave — and we cannot read the result. Not by policy. By math.</small>
---

<div style="background: #0d1117; border-left: 4px solid #00bcd4; padding: 1.5em 2em; margin: 2em 0; border-radius: 8px; color: #e0e0e0;">
<h2 style="color: #00bcd4; margin-top: 0;">Privacy That Can't Be Overridden</h2>
<p>Most apps promise not to look at your data. We made it technically impossible — using your iPhone's Secure Enclave and AWS Nitro Enclaves to ensure your genome stays yours, mathematically.</p>
<p style="margin-bottom: 0;"><a href="/dnavault/about/" style="color: #00bcd4;">Learn how it works →</a></p>
</div>

<!-- Swiper carousel for app screenshots -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>

<div class="swiper dnavault-swiper" style="margin: 2em 0; padding-bottom: 3em;">
  <div class="swiper-wrapper">
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_home.png" alt="Your Genetic Data" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Your Genetic Data</strong><br><small>WGS, AncestryDNA, or 23andMe — stored locally on your device.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_ancestry.png" alt="Ancestral Origins" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Ancestral Origins</strong><br><small>Trace your paternal and maternal lineage back thousands of years.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_health.png" alt="Health Insights" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Health Insights</strong><br><small>81 ACMG genes, pharmacogenomics, and clinically significant variants.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_kinship.png" alt="Kinship Analysis" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Kinship Analysis</strong><br><small>End-to-end encrypted proximity sharing. Nothing retained after analysis.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_kinship_results.png" alt="Precise Results" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Precise Results</strong><br><small>IBD segment analysis identifies Half Siblings, Cousins, Parent/Child, and more.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_ask.png" alt="Ask Your Genome" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Ask Your Genome</strong><br><small>Plain-language questions answered by Claude AI using your local genome.</small></p>
    </div>
  </div>
  <div class="swiper-pagination"></div>
  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>
</div>

<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
<script>
  new Swiper('.dnavault-swiper', {
    slidesPerView: 1,
    spaceBetween: 30,
    centeredSlides: true,
    loop: true,
    pagination: { el: '.swiper-pagination', clickable: true },
    navigation: { nextEl: '.swiper-button-next', prevEl: '.swiper-button-prev' },
    breakpoints: {
      640:  { slidesPerView: 2 },
      1024: { slidesPerView: 3 }
    }
  });
</script>
