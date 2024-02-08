+++
title = '10T RNA-Seq old batch'
date = 2024-02-08T12:46:27-05:00
draft = false
description = " "
tags = ["10T","RNA-seq"]
projects = ["pericentromeric satellites"]
+++
# 10T RNA-seq data analysis
### data
- bam file path: `/project/6007495/shareroot/projects/cell_lines/10Ts/RNAseq/checkout/OLD/C3H10T1/`
- converted to fastq and realigned
- used a diff. RNA-seq kit
### nomenclature
- GSAT_MM:Satellite:Satellite: major satellite
- SYNREP_MM:Satellite:Satellite: minor satellite
## 1. Alignemnt-based quantification
## 1.1 Methods and tools
- aligner: STAR
- quantificaiton: TEcount from TEtranscript
- reference: mm39, mm39.gencode.vM33.annotation.gtf, repeatmasker track from https://labshare.cshl.edu/shares/mhammelllab/www-data/TEtranscripts/TE_GTF/
## 1.2 DE analysis
- genes/TEs with raw count <= 10 in half of the smaples were filtered
- contrast design: `~genotype` KOs vs WT
### 1.2.1 Sample clustering
![olddiff_pca](assets/olddiff_pca.png)
![olddiff_sample-distance-heatmap](assets/olddiff_sample-distance-heatmap.png)



### 1.2.2 Volcano plots of all genes/TEs/Sats
```
- extreme p-values...
```
![](assets/17074172782908.jpg)



### 1.2.3 Volcano plots of TEs/Sats only
![](assets/17074173846563.jpg)
