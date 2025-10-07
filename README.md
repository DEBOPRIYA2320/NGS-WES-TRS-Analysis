# 🧬NGS WES/TRS Analysis
This repository provides a comprehensive **Next-Generation Sequencing (NGS)** workflow designed for **Whole Exome Sequencing (WES)** and **Targeted Region Sequencing (TRS)** analysis — from raw FASTQ files to annotated variant calls.  

---

## 📖 Overview

The project explains and demonstrates:
- Differences between **WGS**, **WES**, and **TRS**
- Metadata identification in **NCBI SRA**
- Quality Control and read pre-processing  
- Alignment, variant calling, and annotation steps  
- Handling **target region (BED)** files  
- Clinical interpretation of **VCF outputs**

---

## 🧩 Tools Used

| Step | Tool | Purpose |
|------|------|----------|
| Raw QC | **FastQC** | Assess sequencing quality |
| Trimming | **Trim Galore** | Remove adapters & low-quality bases |
| Alignment | **BWA** | Map reads to reference genome |
| BAM Processing | **SAMtools** | Sort, index, and manage alignments |
| Variant Calling | **GATK** | Detect SNPs and indels |
| Annotation | **SnpEff** | Predict functional and clinical impact |

---

## 🧠 Workflow Summary

1. **Raw Data QC** → FastQC  
2. **Trimming & Filtering** → Trim Galore  
3. **Alignment** → BWA  
4. **Post-processing** → SAMtools (sort, index, mark duplicates)  
5. **Variant Calling** → GATK (HaplotypeCaller)  
6. **Annotation** → SnpEff  
7. **Interpretation** → Prioritize variants within target regions (using BED files)  

---

## 💡 Key Concepts

- **WGS vs WES vs TRS** – Understanding scope, depth, and cost  
- **Target BED Files** – Define genomic intervals for exome/panel analysis  
- **Coverage Analysis** – Assess sequencing depth and breadth  
- **Clinical Variant Reporting** – Use ClinVar, OMIM, COSMIC references  

---

## 🧰 Skills Highlighted

- NGS Data Pre-processing  
- Variant Detection and Annotation  
- Workflow Optimization for Exome/Panel Data  
- Familiarity with GATK Best Practices  
- Genomic Data Interpretation  

---

# 📑 Project Report

## 1️⃣ Introduction
Next-Generation Sequencing (NGS) has transformed genomics by enabling fast, cost-effective sequencing of DNA and RNA. Among NGS approaches, **Whole Exome Sequencing (WES)** and **Targeted Region Sequencing (TRS)** are powerful methods for identifying variants within coding or specific genomic regions.  
This project focuses on the **bioinformatics workflow for WES/TRS**, outlining key computational steps and tools used for transforming raw sequencing reads into biologically meaningful variant annotations.

---

## 2️⃣ Objectives
- To perform quality assessment and preprocessing of NGS reads.  
- To align reads to a reference genome and generate BAM files.  
- To identify variants (SNPs and indels) using GATK and SAMtools.  
- To annotate variants using SnpEff and interpret their biological significance.  
- To compare workflows and outputs for WGS, WES, and TRS data.

---

## 3️⃣ Materials and Methods

### Tools and Software Used
| Step | Tool | Description |
|------|------|-------------|
| Quality Check | **FastQC** | Evaluate raw sequence quality |
| Trimming | **Trim Galore** | Remove low-quality bases and adapters |
| Alignment | **BWA** | Map reads to reference genome |
| Post-Processing | **SAMtools** | Sort, index, and manage BAM files |
| Variant Calling | **GATK HaplotypeCaller** | Identify SNPs and indels |
| Annotation | **SnpEff** | Predict variant effects on genes/proteins |

### Workflow Overview
1. **Input Data:** Raw paired-end FASTQ files  
2. **Quality Control:** Evaluate read quality using FastQC  
3. **Read Trimming:** Remove adapters and low-quality sequences  
4. **Alignment:** Map reads to reference genome using BWA  
5. **Sorting & Indexing:** Organize and index BAM files  
6. **Variant Calling:** Detect genomic variants using GATK  
7. **Annotation:** Use SnpEff to classify and interpret variant impacts  

---

## 4️⃣ Results and Discussion
- High-quality reads were confirmed using FastQC before and after trimming.  
- Alignment achieved high mapping efficiency with minimal read loss.  
- Variant calling identified SNPs and small indels within targeted regions.  
- SnpEff annotation provided functional classification of variants (e.g., synonymous, missense, nonsense).  
- The workflow effectively demonstrates how **bioinformatics pipelines** translate raw NGS data into meaningful genomic insights.  

---

## 5️⃣ Conclusion
This project successfully demonstrates a **comprehensive NGS workflow** for WES and TRS analysis.  
The integration of multiple open-source tools ensures reliable variant discovery, annotation, and biological interpretation.  
Such workflows are essential for genomic research, clinical diagnostics, and precision medicine.  

---
## 📄 Project Report
You can view the complete project report here:https://github.com/DEBOPRIYA2320/NGS-WES-TRS-Analysis/blob/ac8d517bd6ba9b9dabdf7e66be21c139fe3b2c38/NGS%20-%20Genomics%20data%20analysis%20(Debopriya).pdf
## 📫 Contact
**Author:** Debopriya  
📧 [debopriya0920@gmail.com](mailto:debopriya0920@gmail.com)  
🔗 [GitHub](https://github.com/DEBOPRIYA2320)  
🔗 [LinkedIn](https://www.linkedin.com/in/debopriya2320)

---

## 🧾 License
This project is licensed under the **MIT License**.

---

⭐ *If you found this project helpful, please give it a star on GitHub!*
