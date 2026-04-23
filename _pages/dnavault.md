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

feature_row:
  - image_path: /assets/images/dnavault_home.png
    alt: "Your Genetic Data"
    title: "Your Genetic Data"
    excerpt: "Import WGS, AncestryDNA, or 23andMe — all stored locally on your device. Blood type, sex, ancestry, and quality metrics at a glance."

  - image_path: /assets/images/dnavault_kinship.png
    alt: "Kinship Analysis"
    title: "Kinship Analysis"
    excerpt: "Compare genomes with someone nearby using end-to-end encrypted proximity sharing. No data leaves your devices."

  - image_path: /assets/images/dnavault_kinship_results.png
    alt: "Precise Results"
    title: "Precise Results"
    excerpt: "IBD segment analysis identifies Half Siblings, Cousins, Parent/Child, and more — with haplogroup confirmation."

feature_row2:
  - image_path: /assets/images/dnavault_ancestry.png
    alt: "Ancestral Origins"
    title: "Ancestral Origins"
    excerpt: "Trace your paternal (Y-DNA) and maternal (mtDNA) lineage back thousands of years using Yleaf and mitoLEAF classification."
    url: /dnavault/references/
    btn_label: "Scientific References"
    btn_class: "btn--inverse"

  - image_path: /assets/images/dnavault_health.png
    alt: "Health Insights"
    title: "Health Insights"
    excerpt: "Scan 81 ACMG secondary finding genes, pharmacogenomics, and clinically significant variants. Results stay on your device."

  - image_path: /assets/images/dnavault_ask.png
    alt: "Ask Your Genome"
    title: "Ask Your Genome"
    excerpt: "Plain-language questions answered using Claude AI with direct access to your local genome. 30 days free, then $2.95/month or $19.95/year."
---

{% include feature_row %}

{% include feature_row id="feature_row2" %}

---

## Privacy That Can't Be Overridden

Most apps promise not to look at your data. We made it technically impossible.

**Here's exactly how it works:**

1. **Your phone generates a public/private keypair.** The private key lives in the iPhone Secure Enclave — it never leaves your device, ever.

2. **Your genomic data is processed inside an AWS Nitro Enclave.** Nitro Enclaves are isolated compute environments with no persistent storage, no network access, and no operator access — not even from AWS or StarfleetBio. The enclave's identity is cryptographically attested before it receives any data.

3. **The result is encrypted with your public key** inside the enclave, before it leaves. Only the holder of the private key — you, on your phone — can decrypt it.

4. **We receive ciphertext we cannot read.** Not with our master keys, not in response to a subpoena, not under any circumstance. The mathematics of public-key cryptography makes decryption without your private key computationally infeasible.

This is not a privacy policy. It is a cryptographic guarantee.

---

## Pricing

| | |
|---|---|
| **App purchase** | $2.95 |
| **All on-device features** | Free forever |
| **Ask AI — first 30 days** | Free |
| **Ask AI — Monthly** | $2.95/month |
| **Ask AI — Annual** | $19.95/year |

---

## Legal

- [Privacy Policy](/dnavault/privacy/)
- [Terms of Use](/dnavault/terms/)
- [Scientific References](/dnavault/references/)

Questions? [dnavault@starfleetbio.com](mailto:dnavault@starfleetbio.com)
