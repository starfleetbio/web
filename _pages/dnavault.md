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
  Your genome. Your privacy. Your phone.<br>
  <small>Other apps sell you reports — which means they read your data. When we determine your Whole Genome Sequence, it happens inside a cryptographically attested enclave and the result is encrypted with a key only your phone holds — nobody can read it but you. All analysis — Kinship, Origins, Health, Ask — runs on your phone. This is a cryptographic guarantee, not a privacy policy.</small>
---

<!-- Swiper carousel for app screenshots -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css"/>

<div class="swiper dnavault-swiper" style="margin: 2em 0; padding-bottom: 3em;">
  <div class="swiper-wrapper">
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_welcome.png" alt="Welcome" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>DNAVault</strong><br><small>Your genome. Your privacy. Your phone.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_home.png" alt="Your Genetic Data" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Your Genetic Data</strong><br><small>WGS, AncestryDNA, or 23andMe — stored locally on your device.</small></p>
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
      <img src="/assets/images/dnavault_ancestry.png" alt="Ancestral Origins" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Ancestral Origins</strong><br><small>Trace your paternal and maternal lineage back thousands of years.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_health.png" alt="Health Insights" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Health Insights</strong><br><small>81 ACMG medically actionable genes, pharmacogenomics, and clinically significant variants.</small></p>
    </div>
    <div class="swiper-slide">
      <img src="/assets/images/dnavault_ask.png" alt="Ask Your Genome" style="border-radius:20px; width:100%; max-width:280px; display:block; margin:0 auto; box-shadow: 0 8px 30px rgba(0,0,0,0.3);">
      <p style="text-align:center; margin-top:1em;"><strong>Ask Your Genome</strong><br><small>Ask plain-language questions about your genome — answered on your phone.</small></p>
    </div>
  </div>
  <div class="swiper-pagination"></div>
  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>
</div>

<script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
<script>
  new Swiper('.dnavault-swiper', {
    initialSlide: 0,
    slidesPerView: 1,
    spaceBetween: 30,
    pagination: { el: '.swiper-pagination', clickable: true },
    navigation: { nextEl: '.swiper-button-next', prevEl: '.swiper-button-prev' },
    breakpoints: {
      640:  { slidesPerView: 2 },
      1024: { slidesPerView: 3 }
    }
  });
</script>
