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

The single cell data that these notebooks use are large and so are not deposited
into the git repo directly.  To get the data, you need to go to the Gene Expression
Omnibus. There are three datasets these notebooks use, (1) raw counts from a single lung
sample, (2) fully processes cell by gene matrix with all aggregated samples, and (3) the
metadata file annotating all the cell types and clusters.

Download dataset (1) at https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSM5226581
Scroll down to the bottom and download the http version of `GSM5226581_L01cov_raw_counts.csv.gz`

Download dataset (2) at https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE171524
Scroll down to the botomm and download the http version of `GSE171524_processed_data.csv.gz`

Download dataset (3) at https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE171524
Scroll down to the bottom and download http version of `GSE171524_lung_metaData.txt.gz`

Deposit these datasets into your `veme` folder that was just cloned. Please DO NOT uncompress
these datasets.  They will be uncompressed in memory when analyzing.

## Running this Work

Assuming you have `Juypter Lab` installed on your machine, in the `veme` folder run ...
	
	source env_setup.sh
	Juypter Lab