# VEME Single Cell RNA-Seq Analysis

## Introduction

This respository provides the Jupyter Notebooks for analyzing the single cell RNA-seq data
produce by Melms et al. in https://www.nature.com/articles/s41586-021-03569-1.  This study
analyzes lung tissue in patients who passed from COVID-19 and analyzes immune response 
at a cellular level.

## Accessing this Folder

Assuming you have `git` installed on your machine, in your terminal run ...
	
	git clone https://github.com/zwallace425/veme
	cd veme

## Acquiring the Data

To get the original scRNA-seq data, you need to go to the Gene Expressio Omnibus. There 
are three datasets use to analyze from GEO, (1) raw counts from a single lung sample, (2) fully 
processes cell by gene matrix with all aggregated samples, and (3) the metadata file annotating 
all the cell types and clusters.

Dataset (1) --- https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM5226581
Scroll down to the bottom and download the http version of `GSM5226581_L01cov_raw_counts.csv.gz`

Dataset (2) --- https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE171524
Scroll down to the botomm and download the http version of `GSE171524_processed_data.csv.gz`

Dataset (3) --- https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE171524
Scroll down to the bottom and download http version of `GSE171524_lung_metaData.txt.gz`

### Downsampled Data

To accomidate for lack of memory on certain machines, such as the Virtual Machines used in
the VEME workshop, we have a downsampled version of the cell x gene expresion matrix in a 
Google Drive:

Downsampled Data --- https://drive.google.com/file/d/1cJPAidSgQHPNYDbnHvk3Ob7WuMcbK9mI/view
Download this dataset from the Google Drive

Deposit these datasets into your `veme` folder that was just cloned. Please DO NOT uncompress
these datasets.  They will be uncompressed in memory when analyzing.

## Running this Work

Assuming you have `Juypter Lab` installed on your machine, in the `veme` folder run ...
	
	source env_setup.sh
	Juypter Lab