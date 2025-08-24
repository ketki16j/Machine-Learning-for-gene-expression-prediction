##Predicting Gene Expression from Sparse Genome-Wide SNP Data

This project explores large-scale machine learning approaches to predict gene expression directly from genotype information.

##Introduction

We analyzed millions of SNPs obtained through whole-genome sequencing (WGS) to estimate gene expression levels. Because SNP datasets are typically sparse, we tested four machine learning methods that are well-suited for high-dimensional data: Ridge regression, Lasso regression, Elastic Net (ENET), and Random Forest. To improve prediction performance, we also compared models with and without filtering SNP predictors based on their genomic distance to the target gene and their correlation with expression.

##Dataset

The analysis used data from the Geuvadis Consortium, which includes 462 unrelated human lymphoblastoid cell line samples representing five populations from the 1000 Genomes Project:

CEPH (CEU)

Finns (FIN)

British (GBR)

Toscani (TSI)

Yoruba (YRI)

Details of the dataset:

mRNA expression data: 462 samples

miRNA expression data: 452 samples

Genotype data: 421 samples from 1000 Genomes Phase 1 and 41 from Phase 2

##Data Structure

Expression data: RPKM (Reads Per Kilobase of transcript per Million mapped reads)

Genotypes: VCF (Variant Call Format)

Data Access

Data were downloaded from the European Bioinformatics Institute (EMBL-EBI):

Gene expression files:
GD462.GeneQuantRPKM.50FN.samplename.resk10.txt.gz (86.6 MB)

Genotype files (Chromosomes 1–22, total size ~44.6 GB):
VCF Files
