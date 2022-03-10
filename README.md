# BMW scRNAseq COO 2022 
Practical on dimensionality reduction and single cell RNA sequencing (scRNAseq) data analysis for the course **BMW20421 2021-2022 Bio-informatica** at the Utrecht University 

## Principle component analysis using prcomp()
Even though dimensionality reduction methods are already integrated in the Seurat pipeline, I would like you to gain a bit more insight into how the actual code for  parts of the analysis looks like. Thus, we will start by performing Principle component analysis (PCA) on single cell data using the prcomp() function, which is part of the ‘stats’ package that is an integral component of R. We will visualise the results using ggplot2 and factoextra packages

#### Sections
	3.1 calculate the PCA
	3.2 Visualise the variation explained by PCs
	3.3 Check top contributors to each PC
	3.4 plot the PCA results
	
## Single cell RNA sequencing data analysis using Seurat
In this practical you will learn how to perform analyse scRNAseq data. For this, we will use the well established Seurat pipeline. This pipeline include function that do most of the work ‘behind the scenes’. This makes the tool very user friendly and suitable for todays tutorial. There is extensive documentation on the use of the pipeline. 

#### Sections
	4.1 Downsize the dataset
	4.2 QC metrics
	4.3 Filter low quality cells
	4.4 Normalise
	4.5 Detection of variable genes across the single cells
	4.6 Scale the data and get rid of the confounders
	4.7 PCA analysis
	4.8 Find clusters using SNN Graph Construction and the louvain algorithm
	4.9 UMAP and t-SNE analysis

