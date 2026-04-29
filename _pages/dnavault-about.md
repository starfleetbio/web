---
title: "About"
layout: single
permalink: /dnavault/about/
dnavault_site: true
show_date: false
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/header.jpg
  overlay_filter: 0.4
  overlay_color: "#0D1117"
---

## What is DNAVault?

DNAVault is a privacy-first genomics app for iPhone. It lets you explore your own genetic data — kinship, ancestry, health, and more — entirely on your device. Your genome never leaves your phone without your knowledge, and what does leave is encrypted so that only you can read it.

## Privacy Architecture

Most apps promise not to look at your data. DNAVault makes it technically impossible.

1. **Your phone generates a public/private keypair.** The private key lives in the iPhone Secure Enclave and never leaves your device — ever.

2. **Genomic data is processed inside an AWS Nitro Enclave** — an isolated compute environment with no persistent storage, no network access, and no operator access. Not even StarfleetBio can see inside. The enclave's identity is cryptographically attested before receiving any data.

3. **The result is encrypted with your public key** inside the enclave, before it leaves. Only you — the holder of the private key on your iPhone — can decrypt it.

4. **We receive ciphertext we cannot read.** Not with any master key, not in response to a subpoena, not under any circumstance.

This is not a privacy policy. It is a cryptographic guarantee.

**On-device analysis:**
- **Kinship** — IBD segment comparison runs locally. Proximity sharing is end-to-end encrypted; nothing is retained after analysis.
- **Haplogroup classification** — Y-DNA and mtDNA classification using Yleaf and mitoLEAF, on-device.
- **Health screening** — ClinVar variant lookup runs against a local database you download once.
- **Ask** — Only the text of your question is sent to an AI via an anonymizing proxy. Raw genome data is never transmitted.

## Supported Formats

| Format | Coverage |
|---|---|
| Whole Genome Sequencing (WGS) | Full variant coverage |
| AncestryDNA raw data | ~700K SNPs |
| 23andMe raw data (v3, v4, v5) | ~600K–1M SNPs |

## The Science

DNAVault implements peer-reviewed algorithms for every analysis. See the full [Scientific References](/dnavault/references/) for citations covering kinship, haplogroup classification, health variant interpretation, and ancestry.

## Pricing

| | |
|---|---|
| **App purchase** | $2.95 |
| **All on-device features** | Free forever |
| **Ask AI — first 30 days** | Free |
| **Ask AI — Monthly** | $2.95/month |
| **Ask AI — Annual** | $19.95/year |

## Legal

- [Privacy Policy](/dnavault/privacy/)
- [Terms of Use](/dnavault/terms/)
- [Scientific References](/dnavault/references/)

## Who Built This?

DNAVault is developed by [StarfleetBio](https://starfleetbio.com) — a company focused on computer-aided science for modern research and development.

Questions or feedback: [dnavault@starfleetbio.com](mailto:dnavault@starfleetbio.com)
