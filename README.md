# Data Science | Final Project | Group 02
# Identify epigenetic alterations associated with Alzheimer’s disease and classification of gene expressions between healthy and sick patients
**Christina Kirschbaum, Pushpa Koirala, Melika Moradi**

## Our Project

Alzheimer's disease is the most prevalent kind of dementia and a fatal brain ailment. 
More study into this illness might lead to a better understanding of the condition and more effective treatment options. 
This projects aim is to analyze publicly available RNA-seq and ChIP-seq data from human brain samples 
in order to build a machine learning model that accurately predicts the presence or absence of Alzheimer's disease.

Our project is inspired by the paper Nativio R, Lan Y, Donahue G et al. ["An integrated multi-omics approach identifies
epigenetic alterations associated with Alzheimer’s disease."](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8098004/)


## Data

The data for this project will be taken from GEO, [Series GSE153875](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE153875), for the ChIP-seq data and the raw RNA-seq data as well as the count matrix [Series GSE159699](https://www.ncbi.nlm.nih.gov/Traces/study/?acc=PRJNA670209&o=acc_s%3Aa). 

This includes ChIP-seq data for H3K27ac, H3K9ac, H3K122ac and H3K4me1 as well as RNA-seq data from the
from the lateral temporal lobe of the human brain for eight young healthy patients, ten old heathy patients and twelve patients with Alzheimer's disease.
The samples are from mainly male patients.

The RNA count matrices and the corresponding metafiles can be found in the folder 
[data](https://github.com/nepsygirl/DataScience_finalProjekt_Group2/tree/main/data)
as well as the gene_summary.txt that is needed for the Machine Learning with RNA using Random Forest and SVM.

The count matrices for the ChIP-seq datasets, the npz files generated for the ChIP-seq datasets with `multiBigWigSummary` of deeptools and 
the bed files of the ChIP-seq datasets can be found in the following [Google Drive](https://drive.google.com/drive/folders/1xbMaWXJ4Y3V-Mbgpk7QPJ8Ei1wpMmPTs?usp=sharing),
because they were to big to upload them into this repository.

If you want to work with the BigWig files of the ChIP-seq data, please download them directly from 
[GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE153875).

If you want to work with the FASTQ files of the RNA-seq data, please download them directly from 
[SRA Run Selector](https://www.ncbi.nlm.nih.gov/Traces/study/?acc=PRJNA670209&o=acc_s%3Aa).


## How to run the code

In this repository, we provide a Jupyter notebook and a R markdown file with all the code needed to rerun our project.

In the R notebook, you find the RNA Analysis, the ChIP-seq Analysis with ChIPseeker, the Funtional Enrichment 
and the Machine Learning for hierachical Clustering with RNA.

To run it, the packages ... are needed and the files ...

In the python notebook, you find the Data Integration, the RNA Preprocessing, the Quality Control and the needed conversion, 
the ChIP-seq Analysis with deeptools and the code to generate the ChIP-seq count matrices.
All of these processes run through the Terminal and have been integrated with the package subprocess into Python.
Additionally, it includes the Machine Learning for Random Forest and SVM with the package scikit-learn.

To run it, an environment with ... is needed and the files ...

*Please keep in mind that you may need to change the paths.*
