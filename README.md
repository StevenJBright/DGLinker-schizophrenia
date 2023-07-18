# DGLinker-schizophrenia
A repository for all the code investigating novel disease-associated genes for schizophrenia with the DGLinker webserver (Hu et al., 2021).

Analyses were undertaken by Steven Bright, with supervision from Dr Alfredo Iacoangeli and Jiajing Hu.

## Scripts breakdown
### Figures
This script contains the code for creating all the figures, including:
- Overlap of predicted gene sets
- Overlap of input gene sets
- Stacked bar chart showing the frequency of predicted genes that are in at least one other input list or not

### Filtering SNPs
This script contains the code for mapping the SNPs in Trubetskoy et al.'s (2022) GWAS summary statistics to each of the predicted gene sets. This resulted in five filtered GWAS summary statistics files being created, which were each uploaded to FUMA's SNP2GENE tool to map the prioritised SNPs to genes.

### Functional validation
This script contains the code for identifying the top 20 Revigo-grouped biological processes for each of the predicted gene sets. The result is a single Excel file summarising all the results ranked by enrichment score.

### GWAS validation
This script contains the code for identifying the novel validated genes for each of the predicted gene sets after they have been mapped to genes using FUMA's SNP2GENE tool (see 'Filtering SNPs' script). It also contains the code for preparing the text files used to perform gene-set analysis with each of the predicted gene sets.

### Predicted_genes_DGLinker_vs_bed_files
This script contains the code for exploring the predicted genes listed by DGLinker for each submission and the associated BED files that DGLinker provides for these genes. The two did not perfectly overlap, which this script sought to explore.

### Predicted genes summary
This script contains the code for summarising which input genes were used for each list and which genes were predicted by each list.
