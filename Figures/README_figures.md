# BIOMI6300_IronMicrobiotaProject
16S analysis project for BIOMI6300
 
# Folder Purpose
This directory contains all figures generated during the bioinformatics workflow for the Iron and Gut Microbiota Project. Figures were exported from RMarkdown and organized by analysis steps to improve consistency.

# Structure of the figure folders:
```text
Figures/
│── 00_QC/
│   ├── preQC_aggregate_quality_profiles.png
│   │   # Aggregate forward/reverse read quality before trimming and filtering.
│   ├── postQC_aggregate_quality_profiles.png
│   │   # Aggregate read quality after trimming/filtering.
│   └── PostQC_check.png
│       # Post-filter QC check confirming filtered reads are suitable for ASV inference.
│
│── 02_AssignASVs/
│   ├── error reads-1.png
│   │   # DADA2 learned error-rate model for sequencing error estimation.
│   ├── seqlength_per_step.png
│   │   # Sequence/read retention or length changes across ASV-processing steps.
│   ├── plot_ASVLength_raw.png
│   │   # ASV/sequence length distribution before trimming or chimera removal.
│   ├── plot_ASVLength_trimmed.png
│   │   # ASV length distribution after trimming/filtering.
│   ├── plot_ASVLength_NoChimeras .png
│   │   # ASV length distribution after chimera removal.
│   └── depth_richeness.png
│       # Relationship between sequencing depth and observed richness.
│
│── 03_Preprocessing/
│   └── read_depth.png
│       # Sample sequencing depth distribution used to guide preprocessing/filtering.
│
│── 04_Biodiversity/
│   ├── iNEXT_rarefaction_curve.png
│   │   # Rarefaction/extrapolation curve showing sampling completeness.
│   ├── iNEXT_manual_rarefaction.png
│   │   # Manual rarefaction visualization for diversity comparison.
│   ├── Richeness.png
│   │   # Observed richness comparison across samples/groups.
│   └── Alpha_diversity.png
│       # Alpha diversity summary, likely including Hill/Shannon/Simpson metrics.
│
│── 05_Ordination/
│   ├── Seq_depth.png
│   │   # Sequencing depth check before ordination analysis.
│   ├── scaled_seq.png
│   │   # Scaled/normalized sequencing-depth or abundance diagnostic.
│   └── Bray_curtis_plot.png
│       # Bray-Curtis PCoA ordination showing beta-diversity patterns.
│
│── 06_Microbial abundance/
│   ├── top_phyla.png
│   │   # Most abundant phyla across the dataset.
│   ├── top_genera.png
│   │   # Most abundant genera across the dataset.
│   ├── phyla_relative.png
│   │   # Phylum-level relative abundance composition.
│   ├── genera_relative.png
│   │   # Genus-level relative abundance composition.
│   └── diff_abun_genera.png
│       # Differentially abundant genera across comparison groups.
```
