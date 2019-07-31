# GSEA_network_analysis
Automated GSEA network analysis and pathway annotation of RNAseq data

This R pipeline implements a network analysis on the enriched results matrix
generated from a `DESeq2` differential expression analysis derived from a RNAseq
count matrix from mouse or human tissue. Automated community detection of
differentially regulated gene sets is performed, categorizating genes into
singletons and clusters of different size ranges. Automated label generation is
allowed to associate these clusters with biological themes or processes of which
the member gene sets are part of (such as `KEGG`, `Reactome`, and `Biocarta`
pathways), based on a Jaccard index of a given threshold. 

This pipeline accepts an RNAseq count matrix file (or SummarisedExperiment) with
Ensemble IDs (human or mouse) as row names and samples as columns.

This pipeline is an adaptations of the [Enhancing gene set enrichment using networks pipeline by Michael Prummer](https://f1000research.com/articles/8-129/v2)

Prummer M. Enhancing gene set enrichment using networks [version 2; peer review: 2 approved, 2 approved with reservations]. F1000Research 2019, 8:129
(https://doi.org/10.12688/f1000research.17824.2) 
