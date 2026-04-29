# BIOMI6300_IronMicrobiotaProject
16S analysis project for BIOMI6300

# Analysis Files

## 00_FastQC.Rmd

### Purpose:
Initial quality control of raw paired-end FASTQ sequencing reads.

### Main Analyses:
* Imported raw forward and reverse FASTQ files
* Verified paired-end read counts
* Visualized raw sequencing quality profiles
* Evaluated quality decline across read positions
* Checked presence of forward and reverse primer sequences
* Performed trimming/truncation to remove low quality ends and primers

### Key Outcome:
Checked the quality of reading sequences and trimmed to improve read quality for DADA2.

---

## 02_AssignASVs.Rmd

### Purpose:
Generate Amplicon Sequence Variants (ASVs) from filtered reads using DADA2.

### Main Analyses:
* Learned sequencing error models
* Dereplicated reads
* Performed sample inference using DADA2
* Merged paired-end reads
* Removed chimeric sequences
* Constructed raw ASV count table
* Saved count tables for downstream analyses

### Key Outcome:
Produced the ASV abundance table. 

---

## 03_Preprocessing.Rmd

### Purpose:
Prepare ASV data and metadata for ecological analysis.

### Main Analyses:
* Imported ASV count table and sample metadata
* Created phyloseq object
* Filtered low-depth / low-prevalence taxa
* Checked sample consistency
* Standardized taxonomy and metadata variables
* Generated cleaned dataset for diversity analyses

### Key Outcome:
Produced a cleaned dataset ready for downstream statistical comparisons. 

---

## 04_Biodiversity.Rmd

### Purpose:
Evaluate within-sample microbial biodiversity (alpha diversity).

### Main Analyses:
* Calculated Hill diversity measures
* Estimated richness, Shannon diversity, and Simpson diversity
* Compared diversity among iron-related treatment groups 
* Visualized distributions using boxplots

### Key Outcome:
Assessed how microbial richness and evenness differed within samples in 2 iron groups.

---

## 05_Ordination.Rmd

### Purpose:
Assess between-sample community differences (beta diversity).

### Main Analyses:
* Calculated ecological distance matrices (mainly Bray-Curtis)
* Performed Principal Coordinates Analysis (PCoA)
* Visualized clustering patterns among groups
* Conducted PERMANOVA to test community composition differences

### Key Outcome:
Determined whether microbiome composition significantly differed across treatment groups. 

---

## 06_Microbial abundance.Rmd
### Purpose:
Compare taxonomic composition and dominant microbes across samples.

### Main Analyses:
* Calculated relative abundances of taxa
* Generated stacked barplots of phylum/genus composition
* Identified dominant taxa across groups
* Examined top ASVs contributing to observed patterns
* Interpreted taxa associated with iron-related conditions

### Key Outcome:
Identified microbial genera and ASVs potentially associated with iron supplementation responses.

# Reproducibility
Random generations steps were set seeded. All analyses were performed in **RMarkdown** with version-controlled scripts. Final package versions can be reproduced using:
```r
devtools::session_info()
```

