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

**AncestryDNA or 23andMe** — Import your existing raw data file directly. SNP arrays capture 600K–750K positions — about 15% of a full genome — which is sufficient for Kinship. Origins depends on your array version and sex: AncestryDNA V1 has no mitochondrial positions so maternal lineage (M) is unavailable, and paternal lineage (Y) requires male sex. Health and Ask results are accurate for what's covered, but many clinically significant variants fall outside array coverage. Note that AncestryDNA and 23andMe have already processed your genetic data on their servers; DNAVault cannot retroactively guarantee privacy for data those companies hold.

**BYO WGS via consulting** — If you already have your WGS, [StarfleetBio](https://starfleetbio.com) can help you obtain a WGS file for use with DNAVault through consulting services. WGS provides full variant coverage for Kinship, Origins, Health, and Ask. Note that third-party sequencing happens outside a cryptographic enclave; DNAVault cannot retroactively guarantee privacy for data those providers hold.

**Coming soon: Order WGS from your phone** — We will soon provide the ability to order Whole Genome Sequencing directly from DNAVault. Sequencing will happen inside a cryptographically attested enclave; the result will be encrypted with a key only your phone holds before it ever leaves. This is the only path to a cryptographic privacy guarantee — nobody, including StarfleetBio, can read your genetic data.

## Privacy Architecture

Other genomics services rely on promises — not to read your data, or to anonymize it first. DNAVault removes the possibility entirely.

1. **Your phone generates a public/private keypair.** The private key lives in the iPhone Secure Enclave and never leaves your device — ever.

2. **Genomic data is processed inside an AWS Nitro Enclave** — an isolated compute environment with no persistent storage, no network access, and no operator access. Not even StarfleetBio can see inside. The enclave's identity is cryptographically attested before receiving any data.

3. **Your genetic data is encrypted with your public key** inside the enclave, before it leaves. Only you — the holder of the private key on your iPhone — can decrypt it.

4. **We store an encrypted file we cannot open.** No key exists on our end — not a master key, not an admin override, not one we could hand over in response to a subpoena.

This is not a privacy policy. It is a cryptographic guarantee.

## How Ask Works

Ask translates plain-language questions about your genetic data into answers — without sending your genome anywhere.

Your question is sent to an AI language model via a proxy that verifies every request comes from a genuine, unmodified DNAVault app using Apple's Secure Enclave cryptography.

The AI routes your question into two types of lookups:

**General scientific questions** — what a gene does, what a condition involves, what a variant means in published research — query public biomedical databases. Only gene names, variant IDs, and disease terms are sent. None of your personal data leaves your phone.

**Personal genomic questions** — whether you carry specific variants, your pharmacogenomic profile, your pathogenic findings — run entirely on your phone against your local genome and the on-device variant database. The AI receives only the structured result (e.g., "0 pathogenic variants found in BRCA1"), never your raw genetic data.

The AI formulates a plain-language answer from these results and returns it to your phone.

**The AI sees:** your question, public scientific context, and structured findings from your phone.
**The AI never sees:** your raw genome, variant calls, or genotypes.

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
