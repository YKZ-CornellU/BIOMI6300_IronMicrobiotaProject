# BIOMI6300_IronMicrobiotaProject
16S analysis project for BIOMI6300

# Iron Supplementation and Murine Gut Microbiota – Amplicon Project

## Dataset and Paper

- **Dataset**: 16S rRNA gene amplicon sequencing data from murine fecal samples under varying dietary iron conditions.
- **Original publication**:  
  - * Initial gut microbiota composition is a determining factor in the promotion of colorectal cancer by oral iron supplementation: evidence from a murine model*  
  - Link: https://doi.org/10.1186/s40168-025-02101-1

## Scientific Question
Does dietary iron intake (amount/dose) significantly alter fecal microbial community composition and structure in healthy control mice, and are these alterations detectable in the fecal microbiota?

Specifically:

1. Does iron supplementation change overall **α-diversity** (within-sample diversity) and **β-diversity** (between-sample community dissimilarity)?
2. Does iron intake shift the **relative abundance** of major bacterial phyla and genera?
3. Are specific taxa differentially enriched or depleted in response to iron levels, as detected by LEfSe?

## Hypotheses

1. **Community structure hypothesis**  
   Increasing dietary iron intake will be associated with significant shifts in overall community structure, reflected in differences in β-diversity between low-iron and high-iron groups.

2. **Diversity hypothesis**  
   Higher iron intake will reduce α-diversity indices (e.g., Shannon, observed ASVs/OTUs) due to selective growth of iron-tolerant or iron-utilizing taxa.

3. **Taxa-specific hypothesis**  
   Iron-rich diets will increase the relative abundance of specific bacterial taxa that benefit from elevated luminal iron (e.g., certain Proteobacteria or pathobionts) and decrease taxa that are more competitive under iron-limited conditions (such as lactobacillus).

4. **Fecal signal hypothesis**  
   These iron-driven changes in the gut microbiota will be robustly detectable in fecal samples, allowing fecal microbiota profiling to be used as a proxy for intestinal community shifts.

## Project Goals
- Import and curate metadata and sequence data.
- Quantify α-diversity, β-diversity, and taxonomic composition under different iron conditions.
- Identify differentially abundant taxa with LEfSe.
- Interpret microbiome changes in the context of iron as both a critical host micronutrient and a key resource for microbial growth.

## Repository Structure (Planned)
- `data/` – Small processed data files or metadata only (no raw fastq files).
- `scripts/` – R or Python scripts for processing, analysis, and plotting.
- `results/` – Summary tables, figures, and intermediate outputs.
- `docs/` – Additional documentation or notes.

> **Important**: Large raw sequence files (e.g., `.fastq`, `.bam`) will **not** be stored in this repository. Please refer to:NCBI accession ID: Bioproject PRJNA1138753 
