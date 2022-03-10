# BMW scRNAseq COO 2022 
## 1. Introduction
Practical on dimensionality reduction and single cell RNA sequencing (scRNAseq) data analysis for the course **BMW20421 2021-2022 Bio-informatica** at the Utrecht University 
## 2. Source data
For today’s tutorial, we will use the scRNAseq atlas of the adolescent mouse cortex published by Saunders et al 2018. This data is extensive and is available at mousebrain.org, which we briefly discussed at the end of hte lecture. There is an online tool with which you can browse the data as well.
#### Sections
	2.1 Load the data
		2.1.1 Download
		2.1.2 Load the Seurat object
	2.2 Shape the data for PCA analysis
		2.2.1 Extract the count table as a dataframe
		2.2.2 Downsize
		2.2.3 Invert
		2.2.4 Scale

## 3. Principle component analysis using prcomp()
Even though dimensionality reduction methods are already integrated in the Seurat pipeline, I would like you to gain a bit more insight into how the actual code for  parts of the analysis looks like. Thus, we will start by performing Principle component analysis (PCA) on single cell data using the prcomp() function, which is part of the ‘stats’ package that is an integral component of R. We will visualise the results using ggplot2 and factoextra packages

#### Sections
	3.1 calculate the PCA
	3.2 Visualise results
		3.2.1 Variation explained by PCs
		3.2.2 Check top contributors to each PC
		3.2.3 Plot the PCA results
	
## Single cell RNA sequencing data analysis using Seurat
In this practical you will learn how to perform analyse scRNAseq data. For this, we will use the well established Seurat pipeline. This pipeline include function that do most of the work ‘behind the scenes’. This makes the tool very user friendly and suitable for todays tutorial. There is extensive documentation on the use of the pipeline. 

#### Sections
	4.1 The dataset
		4.1.1 Downsize the dataset
		4.1.2 Check the metadata
	4.2 QC metrics
		4.2.1 Plot some quality metrics
		4.2.2 Calculate additional QC metrics
		4.2.3 Plot the additional quality metrics
	4.3 Filter low quality cells
	4.4 Normalise
	4.5 Detection of variable genes across the single cells
	4.6 Scale the data and get rid of the confounders
	4.7 PCA analysis
		4.7.1 Perform PCA
		4.7.2 Plot PCA results
	4.8 Find clusters using SNN Graph Construction and the louvain algorithm
		4.8.1 SNN Graph Construction
		4.8.2 Find clusters using the louvain algorithm
	4.9 UMAP and t-SNE analysis

