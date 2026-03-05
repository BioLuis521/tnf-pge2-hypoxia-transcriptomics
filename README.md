# TNF–PGE2–Hypoxia Transcriptomic Analysis

## Project Overview

This project investigates transcriptional responses to inflammatory and hypoxic stimuli in intestinal epithelial cells using publicly available RNA-seq datasets.

The goal is to explore whether **TNF signaling and hypoxia activate overlapping transcriptional programs**, and how **PGE2 modulates this response**.

This analysis was inspired by research studying mechanisms of **treatment resistance to anti-TNF therapy in ulcerative colitis**.

---

## Biological Background

Ulcerative colitis (UC) is a chronic inflammatory disease of the colon characterized by persistent immune activation and epithelial damage.

A central driver of inflammation in UC is **Tumor Necrosis Factor-α (TNF)**, a pro-inflammatory cytokine targeted by biologic therapies.

However, up to **one-third of patients fail to respond to anti-TNF therapy**.

One pathway that may influence treatment response is the **COX-2–PGE2 signaling pathway**, which regulates:

- inflammation
- epithelial regeneration
- wound healing

This project explores how **TNF, hypoxia, and PGE2 interact at the transcriptional level**.

---

## Research Questions

1. Which genes are differentially expressed under **TNF stimulation**?
2. Which genes are regulated by **hypoxia**?
3. Are there **shared transcriptional programs** between TNF and hypoxia?
4. How are these genes affected when **TNF signaling is combined with PGE2**?

---

## Datasets

Two independent RNA-seq datasets were analyzed:

- **Hypoxia dataset** – epithelial transcriptional response to hypoxia
- **Inflammation dataset** – epithelial response to TNF and TNF + PGE2

Both datasets were analyzed using **DESeq2**.

---

## Methods

RNA-seq differential expression analysis was performed in **R** using the following workflow:

1. Differential expression analysis with **DESeq2**
2. Identification of significantly regulated genes
3. Cross-dataset comparison of gene regulation
4. Visualization using heatmaps

Statistical threshold used:

- adjusted p-value (padj) < 0.05

---

## Key Result

A subset of genes upregulated under **TNF stimulation** were also upregulated in **hypoxia conditions**.

These shared genes remained **mostly upregulated under TNF + PGE2 stimulation**, suggesting that PGE2 does not completely suppress the transcriptional program activated by TNF and hypoxia.

---

## Project Structure
# tnf-pge2-hypoxia-transcriptomics
Comparative transcriptomic analysis of TNF, PGE2 and hypoxia responses in intestinal epithelial organoids.

---

## Tools

- R
- DESeq2
- tidyverse
- pheatmap

---

## Future Work

Potential extensions of this project:

- pathway enrichment analysis
- gene ontology analysis
- integration with additional inflammatory datasets
- visualization with PCA and clustering

---

## Author

Luis Patiño  
Biologist | Aspiring Bioinformatician
