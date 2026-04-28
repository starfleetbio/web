---
title: MyDNAVault — Privacy Policy
layout: single
permalink: /dnavault/privacy/
show_date: false
dnavault_site: true
toc: true
toc_label: "Contents"
header:
  overlay_image: /assets/images/header.jpg
  overlay_filter: 0.3
  min_height: 180px
---

*Effective date: March 18, 2026*

## Overview

MyDNAVault is a privacy-first application. **Your genetic data never leaves your device.** All analysis — kinship comparison, haplogroup classification, health variant scanning — runs entirely on your iPhone or iPad. StarfleetBio does not operate servers that receive, store, or process your genomic data.

---

## 1. What Data MyDNAVault Collects

### 1.1 Genomic Data (Local Only)

When you import a raw DNA file (23andMe, AncestryDNA, or a Whole Genome Sequencing database), that data is stored in an encrypted SQLite database on your device. It is never transmitted to StarfleetBio or any third party.

### 1.2 Reference Databases (Bundled)

MyDNAVault includes reference databases used for analysis (Y-DNA haplogroup tree, mitochondrial haplogroup motifs, rsID coordinate bridge). These are bundled with the app and do not require network access.

### 1.3 Health and Variant Queries

When you use the **Ask** or **Health** features, MyDNAVault queries biomedical databases for variant information:

- **ClinVar** queries run entirely on-device against a locally downloaded database. Your genomic variants are never transmitted to NCBI or any external server.
- **BioMCP** variant and trial search queries are routed through a StarfleetBio proxy service, which conceals your device's IP address from the BioMCP service. These queries contain only SNP identifiers (e.g., rsIDs, gene names) — no raw genomic sequences and no personally identifying information.

### 1.4 App Store and Apple Services

Apple may collect analytics and crash reports through standard iOS mechanisms. This data is governed by [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).

### 1.5 Contact and Support

If you contact us by email at [dnavault@starfleetbio.com](mailto:dnavault@starfleetbio.com), we retain your message and email address to respond to your inquiry. We do not add you to any mailing list.

---

## 2. What Data MyDNAVault Does NOT Collect

- Your name, address, or any demographic information
- Your genotype data, VCF files, or raw DNA files
- Device location
- Usage analytics (beyond standard Apple crash reporting)
- Any data from your Contacts, Camera, Microphone, or other device sensors

---

## 3. Data Sharing

StarfleetBio does not sell, rent, or share your data with third parties. The only outbound network requests made by MyDNAVault are the public biomedical API queries described in §1.3, which contain no personal or genomic identifiers.

---

## 4. Data Security

Your genomic database is stored in your device's app sandbox, which is encrypted by iOS using your device passcode. We recommend enabling a strong device passcode and Face ID / Touch ID.

If you delete the MyDNAVault app, all locally stored genomic data is permanently removed from your device.

---

## 5. Children

MyDNAVault is not directed at children under 13. We do not knowingly collect information from children. If you believe a child has used the app in a way that raises privacy concerns, please contact us.

---

## 6. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the effective date at the top of this page. Continued use of the app after a policy change constitutes acceptance of the updated terms.

---

## 7. Contact

For privacy questions or concerns:

**StarfleetBio**
[dnavault@starfleetbio.com](mailto:dnavault@starfleetbio.com)

---

*MyDNAVault is for informational purposes only and is not a clinical diagnostic tool. See our [Terms of Use](/dnavault/terms/) for details.*
