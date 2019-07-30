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
