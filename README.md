# Galaxy Multiomics

This repository contains the R-based scripts for preliminary data analysis and visualization following the [ASaiM pipeline](https://f1000research.com/articles/10-103) in Galaxy. This project, **Multi-omic informatics for characterizing microbiomes and their role in health, disease and environment** was part of the Norwegian Centennial Chair Program, supported by the Norwegian University of Life Sciences (NMBU), the University of Oslo (UiO) and the University of Minnesota (UM).

## Intro
The (metagenomics, metatranscriptomics)[https://www.ncbi.nlm.nih.gov/sra/?term=SRP134228] and (metaproteomics)[https://www.ebi.ac.uk/pride/archive/projects/PXD016242] data from the simplistic microbial community SEM1b were processed with the ASaiM pipeline and the output files were used as input for this analysis.

## Input data
The required files to run the analysis are:
- **gene_map.txt**: maps the ORFs to their respective aliases, assembly contig and metagenomic bin
- **Kallisto_abundances_all.txt**: gene expression table
- **Galaxy303-Protein_Groups.txt**: protein quantification table
- **InterProScan_CAZy_fromGalaxy.txt**: CAZyme annotation of the ORFs

## Output
The analysis produces the aggregated tables according to MT/MP-ORF groups and a summary functional plot per 'omics per bin per functional class.

![alt text](/results/MO_Kegg.pdf)

## Relevant literature
- Mehta S, Crane M, Leith E et al. ASaiM-MT: a validated and optimized ASaiM workflow for metatranscriptomics analysis within Galaxy framework. F1000Research 10:103 (2021). 
- Kunath, B.J., Delogu, F., Naas, A.E. et al. From proteins to polysaccharides: lifestyle and genetic evolution of Coprothermobacter proteolyticus. ISME J 13, 603–617 (2019).
- Delogu, F., Kunath, B.J., Evans, P.N. et al. Integration of absolute multi-omics reveals dynamic protein-to-RNA ratios and metabolic interplay within mixed-domain microbiomes. Nat Commun 11, 4708 (2020).
