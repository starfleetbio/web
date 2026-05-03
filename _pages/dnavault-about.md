---
title: "About"
layout: splash
permalink: /dnavault/about/
dnavault_site: true
show_date: false
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/header.jpg
  overlay_filter: 0.4
  overlay_color: "#0D1117"
excerpt: >
  Your genetic data. Analyzed on your phone.<br>
  <small>DNAVault runs Kinship, Origins, Health, and Ask locally — your genetic data never leaves your phone.</small>
---

## What is DNAVault?

DNAVault analyzes your genetic data on your phone. Import a file from AncestryDNA, 23andMe, or a Whole Genome Sequence and get:

- **Kinship** — verify unrelated, or find relatives and determine your precise relationship — parent/child, siblings, cousins, and beyond
- **Origins** — trace your paternal and maternal lineage back thousands of years
- **Health** — screen 81 medically actionable genes, check for genetic variants linked to inherited conditions, and learn how these affect drug metabolism
- **Ask** — answer plain-language questions about your genetic data

Privacy makes this more powerful. Your genetic data is the most personal data that exists — it never changes, identifies your relatives, and can be used against you by insurers, employers, or governments. Because analysis runs locally on your phone, you can engage with your genetic data fully, without trusting anyone.

This is a cryptographic guarantee, not a privacy policy.

## Genome Sources

There are three ways to bring your genetic data to DNAVault, each with different coverage and privacy tradeoffs.

**AncestryDNA or 23andMe raw data** — Import your existing SNP array file directly. 600K–700K SNP positions are sufficient for Kinship analysis and haplogroup classification. Health screening and Ask provide degraded results compared to WGS — many clinically significant variants fall outside array coverage. Note that AncestryDNA and 23andMe have already processed your genome on their servers; DNAVault cannot retroactively guarantee privacy for data those companies hold.

**BYO WGS via consulting** — StarfleetBio can help you obtain a WGS genome file through consulting services. WGS provides full variant coverage for Health, Ask, and Kinship. As with SNP arrays, third-party WGS sequencing happens outside a cryptographic enclave — your genome passes through third-party infrastructure during processing.

**Coming soon: Order WGS from your phone** — We are building the ability to order Whole Genome Sequencing directly from DNAVault. Sequencing will happen inside a cryptographically attested enclave; the result will be encrypted with a key only your phone holds before it ever leaves. This is the only path to a cryptographic privacy guarantee — nobody, including StarfleetBio, can read your genetic data.

## Privacy Architecture

Other genomics services rely on promises — not to read your data, or to anonymize it first. DNAVault removes the possibility entirely.

1. **Your phone generates a public/private keypair.** The private key lives in the iPhone Secure Enclave and never leaves your device — ever.

2. **Genomic data is processed inside an AWS Nitro Enclave** — an isolated compute environment with no persistent storage, no network access, and no operator access. Not even StarfleetBio can see inside. The enclave's identity is cryptographically attested before receiving any data.

3. **Your genetic data is encrypted with your public key** inside the enclave, before it leaves. Only you — the holder of the private key on your iPhone — can decrypt it.

4. **We store an encrypted file we cannot open.** No key exists on our end — not a master key, not an admin override, not one we could hand over in response to a subpoena.

This is not a privacy policy. It is a cryptographic guarantee.

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
