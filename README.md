# Predicting Gene Expression from Sparse Genome-Wide SNP Data  

This project explores **large-scale machine learning approaches** to predict gene expression directly from **genotype information**.  

---

## 📖 Introduction  

We analyzed millions of SNPs obtained through **whole-genome sequencing (WGS)** to estimate gene expression levels.  

Because SNP datasets are typically **sparse and high-dimensional**, we tested four machine learning methods:  
- Ridge Regression  
- Lasso Regression  
- Elastic Net (ENET)  
- Random Forest  

To improve prediction performance, models were compared **with and without SNP filtering**, based on:  
- Genomic distance to the target gene  
- Correlation with target gene expression  

---

## 📊 Dataset  

The analysis used data from the **Geuvadis Consortium**, which includes **462 unrelated human lymphoblastoid cell line (LCL) samples** from the [1000 Genomes Project](https://www.internationalgenome.org/).  

### Populations  
- CEPH (**CEU**)  
- Finns (**FIN**)  
- British (**GBR**)  
- Toscani (**TSI**)  
- Yoruba (**YRI**)  

### Dataset Details  
- **mRNA expression data**: 462 samples  
- **miRNA expression data**: 452 samples  
- **Genotype data**: 421 individuals from Phase 1 + 41 from Phase 2 of 1000 Genomes  

---

## 📂 Data Structure  

- **Gene Expression**: RPKM (*Reads Per Kilobase of transcript per Million mapped reads*)  
- **Genotypes**: VCF (*Variant Call Format*)  

---

## 🔗 Data Access  

Data were downloaded from the **European Bioinformatics Institute (EMBL-EBI)**:  



