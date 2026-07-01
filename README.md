# Mammary RNA-seq Analysis

## Overview

This repository contains an exploratory RNA-seq analysis of the **SRP045534** dataset using R and Bioconductor packages. The project investigates gene expression patterns in **Basal** and **Luminal mammary epithelial cells** across different stages of mammary gland development.

The analysis includes data exploration, metadata processing, quality assessment, and preparation for downstream differential expression analysis.

---

## Dataset

* **Study:** SRP045534
* **Data format:** `SummarizedExperiment (.rds)`
* **Platform:** Bulk RNA-seq

Developmental stages included:

* Virgin
* Pregnant (18.5 days)
* Lactation (2 days)

Cell populations:

* Basal cells
* Luminal cells

---

## Project Objectives

* Load and inspect RNA-seq count data
* Explore sample metadata
* Extract biological variables from sample annotations
* Summarize experimental design
* Examine sequencing depth across samples
* Assess gene count distributions
* Evaluate gene detection across samples
* Prepare data for downstream differential expression analysis using DESeq2

---

## Software and Packages

The analysis was performed in **R** using the following packages:

* data.table
* dplyr
* tidyverse
* ggplot2
* DESeq2
* edgeR
* clusterProfiler
* readxl

---

## Analysis Workflow

### 1. Data Import

* Load the `SummarizedExperiment` object
* Inspect assays and metadata

### 2. Metadata Processing

Sample titles were parsed to extract:

* Cell type (Basal or Luminal)
* Developmental stage
* Biological replicate

### 3. Raw Count Exploration

* Inspect count matrix dimensions
* Examine count summaries
* Calculate library sizes
* Visualize sequencing depth

### 4. Quality Assessment

Quality control included:

* Library size comparisons
* Gene count distributions
* Log-transformed count distributions
* Detection of zero-count genes
* Number of samples expressing each gene

### 5. Sample Summary

A simplified metadata table was generated containing:

* Cell type
* Developmental stage
* Replicate
* Library size

---

## Key Analyses

* Metadata extraction from sample annotations
* Library size assessment
* Gene expression distribution
* Detection of lowly expressed genes
* Sample quality summaries

---

## Author
Zainab Fatima & Yousra Dehgane
NGS Project — RNA-seq analysis using R and Bioconductor.

