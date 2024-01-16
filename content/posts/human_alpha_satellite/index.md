+++
title = 'Human Alpha Satellite'
date = 2024-01-15T11:45:42-05:00
draft = false
description = " "
tags = [
    "ChIP-seq",
    "satellite repeat",
    "cal27",
]
projects = ["pericentromeric satellites"]
+++

## Cell type/line
Head and neck cancer epithelial cells, Cal27.

## Method
- `deeptools ComptueMatrix` profiling
- Only kept active HOR; one per chromosome
- More consistent in length
- Most of them > 1.0 mb except the one on chr21
- Body length: 2.0 mb
- Flanking: 2.0 mb each side

## Input and histone marks
### Seletced samples
<center><img src="assets/matrix.cal27_input.2mdist.100kbin.activehor.png" width="70%" /></center>

<center><img src="assets/matrix.cal27_k36me2.2mdist.100kbin.activehor.png" width="70%" /></center>

<center><img src="assets/matrix.cal27_k27me3.2mdist.100kbin.activehor.png" width="70%" /></center>

<center><img src="assets/matrix.cal27_k9me3.2mdist.100kbin.activehor.png" width="70%" /></center>


### All samples
![](assets/Picture1.png)

## IGV screenshot for chr8
<center><img src="assets/Screenshot 2024-01-03 at 13.44.33.png" width="80%" /></center>